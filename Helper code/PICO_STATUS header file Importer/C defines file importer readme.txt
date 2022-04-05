This helper vi generates arrays needed if additions/changes to any of the C PICO_STATUS enum values are changed.
These can then be used copied and used by the error handler in these examples.

Instructions

Run the vi in his folder

You will be prompted to select a file, the PicoStatus.h file is normally located here (64-bit SDK installer)-
C:\Program Files\Pico Technology\SDK\inc\PicoStatus.h

The vi will read the file and generate Arrays (String and U32 values), and ring control for all the #define PICO_STATUS values.

To update the error codes used in these examples do the following-

1) In the block diagram, right click on each array and select "Create Constant" (String and U32 values).

2) Open the vi -  \shared\PicoErrorString.vi and delete each of the array constants. (String and U32 values)

3) Copy each array constant generated from "C defines file importer.vi "to the "PicoErrorString.vi"

4) Rewire each array in the block diagram "PicoErrorString.vi" as before, and save the vi.