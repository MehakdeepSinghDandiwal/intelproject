# intelproject
Design and Functional Simulation of Land rover FIGO FSM. 
You are an engineer working for ISRO. They want you to design an FSM that will test their newest land-rover Figo on their campus. ISRO wirelessly transmits the travel plans to Figo, and then Figo moves according to that information.

To design your FSM, you first select the following locations around the ISRO campus and assign each location with a state in 3-bit binary representation: Room0[000], Room1[001], Room2[ 010], Room3[011], Room4[100], Room5[101], Room6[110], and the Room7[111].

To simplify your test, you inform ISRO to send Figo’s FSM a binary sequence for travel plans (e.g., ‘1-0-0-0-1’ to cause Figo to move five times). In other words, Figo receives either ‘0’ or ‘1’ for each move and travels to the next destination as specified below. Figo starts off at Room0. Design an FSM output of which should give Figo’s current location.



Room0[000]	If 0, stay at Room0	If 1, go to Room1
Room1[001]	If 0, go to Room2	If 1, go to Room4
Room2[010]	If 0, go to Room3	If 1, go to Room4
Room3[011]	If 0, stay at Room3	If 1, go to Room0
Room4[100]	If 0, go to Room7	If 1, go to Room5
Room5[101]	If 0, go to Room3	If 1, go to Room6
Room6[110]	If 0, go to Room7	If 1, stay at Room6


