# PID Control System Project

The goal for this project is to:
* create PID controller for steering wheel
* implement the controller
* tune the Kp, Ki, and Kd parameter until the car always stay inside the lane

## Tuning Strategy

First, I think about what each gain in the PID do.
* Proportional Gain is equal to the current error. Ki will adjust the steering so it's proportional to the error.
* Integral Gain is the sum of all the previous error. Ki will try to minimize the long term error.
* Derivative control use the change from previous error. Kd will prevent oscillating and response time.

Therefore, I set the value of Kp, Ki, and Kd to 10, 5, 20.
However, because the cross track error could have value from -12 to 12 and the steering angle should be between -1 and 1, it cause the car to go out of lane and wasn't to come back fast enough.






I set the limit for the steering angle as wel as lower the parameter down. 

