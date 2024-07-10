
# RUL Prediction Using Multilayer Perceptron Model

With the growing number of EV vehivles, we generate more and more EV batteries. However, Ev batteries are no longer suitable for vehicles once their capacity degrades to ~70%, and must be immediately replaced as they pose a threat to the vehicle and the driver. Current RUL prediction requires heavy machinenary and considerable time, in order to reduce this, a Preemptive effort must be made. Using a CAN BUS on the vehicle and by emplying ML model such as this, we can easily get a rough estimate on the RUL of the Cell.


## Why MLP?

Upon Observing the graphs of Capacity vs Cycle, I saw that they were highly non linear with spikes here and there, as such, MLP is know to perform well in non linear conditions and therefore I chose this model
## Working

We simple analyse the Voltage capacity of each cycle,

calculate the SOC

Covert the SOH to SOC 

 [using the formula given in
 A Novel Prediction Process of the Remaining Useful Life of
 Electric Vehicle Battery Using Real-World Data]

Use LOOCV (leave one out cross validation) due to limited Data
