<summary><strong>Step 2: Marking Functions for Hardware Implementation</strong></summary>

This application has two hardware functions. One hardware function, `mmult`, multiplies two matrices to produce a matrix product, and the second hardware function, `madd`, adds two matrices to produce a matrix sum. These hardware functions are combined to compute a matrix multiply-add function. Both functions `mmult` and `madd` are specified to be implemented in hardware.  

When the SDSoC environment creates the project from a template, it specifies the hardware functions for you. In cases where hardware functions have been removed or have not been specified, follow the steps below to add hardware functions.  

>**:pushpin: NOTE:**  For this lab, you do not need to mark functions for hardware - the template code for matrix multiplication and addition has already marked them. If you don't have the `madd` and `mmult` functions marked as HW Functions, you could do the following to mark them as HW Functions.

  1. The SDx Project Settings window provides a central location for setting project values. Click on the tab labeled lab1 (if the tab is not visible, double-click on the 1 file in the Project Explorer tab) and in the HW functions panel, click on the **Add HW Functions** ![](./images/vvd1517376007004.png) to invoke a dialog to specify hardware functions.  

  2. Ctrl-click (press the Ctrl key and left click) on the `mmult` and `madd` functions to select them in the "Matching elements" list. Click **OK**, and observe that both functions have been added to the hardware functions list.  

     ![](./images/pdl1526589550986.png)  

     Alternatively, you can expand `mmult.cpp` and `madd.cpp` in the Project Explorer, right-click on `mmult` and `madd` functions, and select **Toggle HW/SW** (when the function is already marked for hardware, you will see the function `mmult(float[], float[], float[]): void [H]` in the Project Explorer tab). When you have a source file open in the editor, you can also select hardware functions in the Outline window.  

     ![](./images/kkz1526589743219.png)  

</details>

<details>
