## Analyzing plot

* The Throttle plot shows a little bit of oscilating which may could be dealt with by adjusting the dampaning rate
* The Steering plot shows a big oscilation between extreme Steering angles, this could ether ne due to a false/bad choosen way ob calculating the steering error or a better tuning of the PID is needed

## Answering questions

How would you design a way to automatically tune the PID parameters?:
* In a Simmulation you could exactly calculate what the optimal steering and throttle is by the discribed "twiddle" method. Adjusting one Parameter after the other and look for minimal errors.

PID controller is a model free controller, i.e. it does not use a model of the car. Could you explain the pros and cons of this type of controller?
Find at least 2 pros and cons for model free versus model based:

Pros:
* Can be used on different Vehicles
* Easier to compute

Cons:
* Limited accuracy
* No consideration of environment like snow

