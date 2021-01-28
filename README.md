# Purely Dynamic and Stochastic Vehicle Routing Problem with Delivery Deadlines and Shift Flexibility (PDSVRPDDSF)

Instances for a dynamic and stochastic vehicle routing problem variant as introduced in:

> A Double-Horizon Approach to a Purely Dynamic and Stochastic Vehicle Routing Problem with Delivery Deadlines and Shift Flexibility
> Nikolaus Frohner, Günther R. Raidl
> Proceedings of the 13th International Conference on the Practice and Theory of Automated
> Timetabling - PATAT 2021: Volume I (Patrick De Causmaecker, Ender Özcan, Greet Vanden Berghe, eds.), 2020.
> https://www.ac.tuwien.ac.at/files/pub/frohner-20.pdf

Each instance consists of five files with information regarding order times, positions of depot and the orders, the driver shifts, the hourly expected orders over the day (aka load pattern), and the travel time matrix.

*Order times* consist of availability times (time when the order arrived), release times (time when order can loaded into a vehicle earliest), and a due time (delivering afterwards incurs a quadratic penalty).

*Positions* of the depot and the orders are 2D-coordinates.

*Drivers shifts* are specified via three columns, for each driver the shift start time, the earliest shift end time, and the planned shift end time, after which no route can be started (bu ended).

A *Load pattern* consists of the Poisson means for each hour of the planning horizon, and the probability for an order to be due one hour after its arrival or two hours.

The *Travel time matrix* includes travel times between depot and customers and between customers and additionally stop times to/from customers and loading/manipulation time from/to the depot.

The load patterns are reused over a group of instances and therefore put into a separate directory.