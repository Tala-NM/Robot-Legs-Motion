# Robot-Legs-Motion
This algorithm controls the walking motion of a bipedal robot using six servo motors (three in each leg: pelvis, knee, and foot). 
The goal is to achieve forward motion in a stable and balanced manner.

1. **Initialization:**
   - **Set Initial Servo Positions:** 
     - Start with all servos in a neutral standing position.
     - For standing, set the pelvis servos to 90°, the knee servos to 90°, and the foot servos to 90°. This keeps the robot balanced and upright.

2. **Walking Cycle:**
   - **Repeat the Following Steps Indefinitely:**

   1. **Lift Right Leg:**
      - Adjust the right leg servos to lift the leg off the ground.
      - **Why:** Lifting the leg is essential to move it forward without dragging.
      - **How:** Set the right pelvis to 45° to raise the leg, right knee to 90° to keep the leg straight, and right foot to 45° to tilt the foot upwards.

   2. **Move Right Leg Forward:**
      - Adjust the right knee and foot servos to move the leg forward.
      - **Why:** Moving the leg forward propels the robot ahead.
      - **How:** Gradually increase the right knee to 180° to extend the leg forward and right foot to 90° to prepare for landing.

   3. **Place Right Leg Down:**
      - Lower the right leg to the ground.
      - **Why:** Placing the leg down provides support and balance.
      - **How:** Return the right pelvis to 90° to lower the leg, right knee to 90° to bring the leg down, and right foot to 90° to place the foot flat.

   4. **Lift Left Leg:**
      - Adjust the left leg servos to lift the leg off the ground.
      - **Why:** Similar to the right leg, lifting the left leg allows for forward movement.
      - **How:** Set the left pelvis to 45° to raise the leg, left knee to 90° to keep the leg straight, and left foot to 45° to tilt the foot upwards.

   5. **Move Left Leg Forward:**
      - Adjust the left knee and foot servos to move the leg forward.
      - **Why:** Moving the leg forward continues the walking cycle.
      - **How:** Gradually increase the left knee to 180° to extend the leg forward and left foot to 90° to prepare for landing.

   6. **Place Left Leg Down:**
      - Lower the left leg to the ground.
      - **Why:** Placing the leg down provides support and balance.
      - **How:** Return the left pelvis to 90° to lower the leg, left knee to 90° to bring the leg down, and left foot to 90° to place the foot flat.

   7. **Adjust Balance:**
      - Ensure the robot remains stable and balanced.
      - **Why:** Maintaining balance prevents the robot from tipping over.
      - **How:** Slight adjustments to the pelvis servos may be necessary to keep the robot centered.

   8. **Timing Control:**
      - Introduce appropriate delays between each movement step.
      - **Why:** Delays ensure smooth and coordinated movement.
      - **How:** Use delay functions to create pauses between movements.

