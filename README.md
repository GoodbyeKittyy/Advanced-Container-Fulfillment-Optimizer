## Solution Explained

This "Combiner" created in Flexsim is different from a traditional library accessed Combiner because:

1) You can set how many containers can be packed at a time. By default, 3 cases were packed simultaneously within each cycle. I named these "batches" in my logic. This variable can accessed as a label on the actual 3D model.

2) It assumes that all the flowitems being packed come from the same port, you can't have multiple sources of flowitems or have a recipe. Although it could be modified to allow that.

3) It is very easy to set how many flowitems per container. This variable is accessed as a label on the 3D object. This can be changed easily if the itemtype or some other criteria changes.

4) If the flow of containers or flowitems is delayed, the machine can time out and release a partial batch or partially filled container. I have included a model control GUI so you can manually stop the sources and test this logic. Note the labels associated with max wait time in the object labels again.

5) After a batch of containers and flowitems has been collected, there is a RobotCycleTime that occurs that represents the moving of the flowitems into the containers, this time is ran one time for the entire batch.

While this might not be the final solution for fully automated warehouses, it is a good starting point. The Process Flow is well documented to explain the logic.

Note that this is an Object Process Flow and all instances will need to be connected to the logic in the process flow.

</br></br>

## 3D Animation 

https://github.com/GoodbyeKittyy/Scalable-Pallet-Mole-FIFO-System/assets/161730857/7eb52adb-3627-45a1-8baf-fbd07527a07c

</br></br>

## Model Controls
![Screenshot 2024-04-18 213808](https://github.com/GoodbyeKittyy/Scalable-Pallet-Mole-FIFO-System/assets/161730857/be8c8ecc-855d-4b0f-a532-22eedc1d54b1)

</br></br>

## Live Process Flowcharts

https://github.com/GoodbyeKittyy/Scalable-Pallet-Mole-FIFO-System/assets/161730857/97023085-7313-4ba4-abe9-4aa57071e243
