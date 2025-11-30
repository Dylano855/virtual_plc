Morning Routine PLC Project (TwinCAT 3)

This project implements a simple PLC program in Structured Text (ST) that simulates a morning routine before class.

Overview of the Process

The PLC program represents a normal morning routine:

Wake-Up Task:
1.Idle
2.Alarm rings
3.Get out of bed
4.Brush teeth
5.Routine complete → signals the breakfast task

Breakfast Task:
1.Idle
2.Waiting for wake-up routine to finish
3.Make breakfast
4.Eat breakfast
5.Finished and ready to leave

These two tasks run independently but communicate through global variables.


All diagrams are included as PlantUML files:

WakeUp_StateDiagram.puml – state diagram for the wake-up task

Breakfast_StateDiagram.puml – state diagram for the breakfast task

Tasks_Sequence.puml – communication between tasks

FunctionCall_Sequence.puml – how the function is called


