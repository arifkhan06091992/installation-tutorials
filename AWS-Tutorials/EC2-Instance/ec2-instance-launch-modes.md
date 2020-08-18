### EC2 instance Types
- [On Demand Intances](#on-demand-instances)
- [Reserved Instance](#reserved-instance)
- [Convertible Reserved](convertible-reserved)
- [Schedule Reserve Intances](schedule-reserve-intances)
- [Spot Instances](spot-instances)
- [Dedicated Instances](dedicated-instances)
- [Dedicated Hosts](dedicated-Hosts)


#### On Demand Intances
- We pay for what we use (billed per second after the first minute ).
- it has the highest cost, but there's no upfront payment.
- There's no long term commitment
- Recommended for short-term, uninterrupted work loads where we can't predict how our application will behave.

#### Reserved instances
- Up to 75% discount compared to On Demand Intances
- Pay upfront for waht you use with long term commitment
- Reservation period can be 1 or 3 years
- Reserve a specific instance type
- Recommanded for steady stage usage applicatation ( think database )

#### Convertible Reserved
- Can Change EC2 instance type
- Upto 54% Discount compared to On Demand Intances

#### Schedule Reserve Intances
- Need an instance maybe on every Saturday night during the football game but then you don't need it during the rest of the time

#### Spot Instances
- we can get a discount of up to 90% compared to On Demand
- we have to bid then we get the unit the instance as long as its price
- price will vary based on offer and demand When there's a lot of demand, the price goes up, and when there's a lot, not much demand, the price goes down.
- the Spot instances, they can be lost And so when they're reclaimed, you have a two minute notification So it's, you have to just shut down your work
- when you need basically to do batch jobs for very cheap or big data analysis, or workloads that can fail.

#### Dedicated Hosts
- physical EC2 server for you to use.
- you get the hardware, and you get full control over how the EC2 instance is going to be placed.
- You also get full visibility into the hardware sockets and physical cores, so you have direct access to the CPU.
- 3 year period reservation.
- more expensive, but you get the benefit that you control the hardware in some ways.
- sometimes some vendors have a complicated licensing model, called BYOL ( the Bring Your Own License ) that wanna bill you based on number of cores, number of sockets, or whatever.
- you have a company that has a very strong regulatory or compliance needs and want to make sure that you're the only one on the hardware and no other customer of AWS can be on it as well. 

#### Dedicated Instances
- you still are running your instance on your own hardware Though you don't get control over the hardware
- if other people, and newer accounts launch instances well these instances may end up on the same hardware as well. But it's still only your account.
- then you don't get any control over the instance placements. That means that if you stop and start a EC2 instance, it may move between different hardware.