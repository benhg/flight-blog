# Ben's Flight Blog

To keep myself honest, I've decided to keep my personal notes from each flight I take in a blog, which everyone can see. Hopefully, this will get me in the habit of writing something up every time I take the air. It will also let me share some of the things I learn and formalize my process. Finally, it will serve as the fourth copy of all of my flight info (Behind my official logbook, my in-flight notebook, and ForeFlight on my iPad.)

## Ground Instruction, October 15, 2020

Today, we finished the powerplant chapter, covered the last of the  aerodynamics chapters (sad, I know), then talked mostly about Say Again Please, which is a book about how to properly engage in radio communications.

### Chapter 2B

We started the session by talking about oil systems. Oil systems in airplanes mostly have two purposes (just like in any other engine): lubrication and cooling. However, because airplane engines are mostly air cooled, the cooling effects of oil are much more important than in, say, a motorcar. We talked about oil pressure and temperature next. Essentially, there is an oil temperature gauge, near one of the cylinders, which mmeasures the pressure of oil flowing through the system. There is an oil pressure gauge, upstream of the pump, which measures pressure of the oil system. We talked about various factors that could make oil pressure and temperature not appear correct during operation. There are way too many possibilities to list here, but for some examples: the wrong type of oil could have been put in the engine, there may be not enough oil, the engine may have been working too hard and is now overheating, the oil system may have a blockage in  it, and so on and so on. One final important thing of note is that any improper oil system configuration will eventually become high-temperature and low-pressure. It is important to continually check oil temperature and pressure throughout the flight.

Next up is the cooling system. As previously mentioned, the cooling system is air-cooled. Air enters the engine through an air intake at the top of the cowl, and is forced down through fins on the cylinder heads, and out the bottom of the cowl. The reason the air is pushed top to bottom rather than bottom to top, which would be thermodynamically optimal, is historical in nature. In the past, when airplanes like the ones I fly were carburetted, the carburettor was placed at the bottom. Carburettor icing is a major concern for planes, so they forced hot cooling air past the carburettor to mitigate the risk of carb ice. Now that planes are fuel injected, the design means it makes more sense to continue to cool the same way.

The exhaust system of a light aircraft is incredibly simple. It's basically a small spark-catcher (which they call a muffler, but isn't one) surrounded by a larger sealed tube. This sealed tube is useful so that cabin heat can exist. Air is passed over the muffler and through a heat exchanger which mixes it with cool air so that it is the desired temperature before being sent into the cabin. Airplanes do not have catalytic converters, so there is a lot of CO coming out of the engine, compared to a car. For this reason, a cracked muffler could be very dangerous. If exhaust is smelled inside the cabin, you  should open vents and windows, turn off the heat system, and try to land the plane for service as soon as possible. Carbon monoxide is dangerous.

Next, we talked about propellers. Propellers essentially behave like a small rotating wing, producing a force in the direction we want to fly the plane. The propeller does not have a constant chord angle from the root to the tip of the propeller, Instead, the angle of attack is steeper at the root of the propeller. This is because if it was not the case, there would be a differential torque on various parts of the propeller and it would get bent. The kinds of airplanes I fly (at least for now) have a fixed-pitch propellers. A fixed pitch propeller is exactly what it sounds like. The pitch angle of the propeller does not change. A variable pitch propeller (more accurately described as a constant-speed propeller, for complicated physics reasons [send me a tweet if you want me to explain to you]), uses an engine-oil driven hydraulic system to alter the pitch of the propeller based on situational power demands of the engine. Some time, I fill fly a skywagon or some other plane which has a constant-speed propeller.

The electrical system of airplanes is rather complex. The electrical system is charged by a 24-volt (at idle) alternator, which is then regulated and rectified into a 24-volt DC current by a regulator. All the radios and lights and starter motors and whatever else in the airplane is run off of this 24 volt power, with the notable exception of the ignition magnetos, which have permanent magnets in them and are driven by movement of the engine. They are completley isolated so that the plane can stay in the air if the electrical system goes down. The ammeter of the airplane measures whether the battery is charging or depleting. In  normal flight, the ammeter  should remain zeroish. Upon startup, the ammeter will show a slight positive reading as the battery recharges itself. If you notice a sudden drop in the ammeter, the alternator has probably died, and you should annnounce this on the radio before turning off your avionics bus to save energy in case of an emergency. The plane has a set of circuit breakers which protect the circuitry. Planes used to have fuses, and you needed to carry spare fuses.

### Chapter 3C

This chapter is the last chapter about the aerodynamics of flight, and it covers a lot of things which are essentially glossing-over of some pretty cool differential equations. I would have loved to model some of this stuff in my nuerical models class in college. Maybe I will fire up some openFOAM simulations in my free time. 

Starting out with climbing flight, we basically talked about how the balance of the four forces of flight is not necessarily as one would always expect. For example, in climbing flight, there is a component of thrust which is opposing weight and a component of weight which is opposing thrust. 

The plane has a left-turning tendency. I have noticed this every time I have flown the plane. As a pilot, you have to learn to push on the right rudder to abate the left turning tendency. This left-turning tendency exists mostly for four reasons. The first of these four reasons is the torque of the engine. The engine and propeller turnn in a clockwise direction, which, due to newton's third law of motion (and some vector cross products), ends up with a left-turning tendency. Next up is gyroscopic procession. There's some more complicated mathematics hiding behind this, but basically, when you have a spinning disk, if a force is applied somewhere along the disk, there will be a resultant force ninety degrees off and relatively forward. This can actually lead to a right-turning tendency in a climb attitude, but the plane will never exhibit such a right-turn tendency. This is because the other effects simply outweigh the procession. Next, is p-factor. P-factor is an asymmetric thrust caused by the descending blade of the propeller taking a bigger "bite" out of the air than the ascending blade of the propeller. P-factor is most noticeable when the engine is at full power, like during a climb. Finally, is spiral slipstream. Essentially, air washes off of the propeller in a spiral motion and will end up hitting the tail on the left side of the tail, coming from the left. This will cause a left yaw tendency.

Next, is descendig flight. Descents are much more complex than climbs, simply by virtue of the fact that we are not power-limited in a descent. In fact, it is perfectly possible to descend with no power at all. The plane's tendency to do so can be quantified by its glide ratio. The glide ratio describes the ratio of horizontal distance to vertical distance while the plane is operating with no power. The typical glide ratio for a Cessna is something like 12:1. This means if my cessna is 1 mile in the air, it should be able to glide for 12 miles before it hits the ground. The glide ratio obviously does not take into account wind. A headwind or tailwind can affect your ability to glide as far as you would normally be able to. A plane can glide furthest at the speed called L/Dmax, or best-glide speed. This speed is the speed at which lift per unit drag is minimized. It is the most efficient speed at which to fly the plane. However, there isn't really one "best glide speed", there is in fact a "best glide angle of attack", which depends on weight. The same is true of stall speed, in that there is no such thing as a "stall speed", because stalls occur whenever the agle of the relative wind is higher than the critical angle. This can happen at any variety of speeds depending on flight conditions.

Next, we talked about turning flight. Basically, we turn by using a component of the lift in the direction of the turn. We make a component of lift show up in this direction by banking the plane. The rudder is mostly used to keep the plane coordinated. Adverse yaw occurs when the plane is in an uncoordinated turn. If the inside aileron is raised, then it will create more lift and will end up yawing the plane in the wrong direction. Conversely, overbanking tendency is caused by the outside aileron creating more lift, as it is going faster. The overbanking tendency is most pronounced at low speeds. Rate and radius of turn are related. All things held equal, a slower turnn will lead to a smaller turning radius. Additionally, all things being held equal, a higher bank angle will lead to a smaller radius of turn. The extreme case of this can be seen in airshows where planes push themselves to extreme bank angles, near 90 degrees. Next, we talked about load factor. Load factor is essentially a centrifugal force (which is a fictitious force, I know :) ) caused by the inertia of the airplane. It is dependent on bank angle. For example, at 60 degrees, the airplane will experience a load factor of 2 Gs. This goes to infinity as bang angle approaches 90  degrees. Finally, we talked about maneuvering speed and the operating envelope. The operating envelope is the set of pairs of load factor and speed at which the airplane can operate without stalling and without sustaining damage due to excessive load factor. Maneuvering speed is a specific point on the envelope, where any increase in bank angle would cause a stall, and any increase in speed would cause physical damage to the airplane's wings. It is dependent on weight the same way that best-glide speed is. Remember, there is no such thing as a "stall speed", because stalls occur whenever the agle of the relative wind is higher than the critical angle. This can happen at any variety of speeds depending on flight conditions.

## Flight 6: October 10, 2020

Today, i had a good flight. A lot of practice with things I have previously tried, as well as learning a couple of new things.

### Ground, Pre-flight:


Before the flight, I did the weather briefing, checked flight restrictions, and set up my notebook. We planned to practice turning stalls and approach-to-land stalls. An approach-to-land stall is, as the name suggests, a stall that occurs when the plane is configured for approach-to-land. To do an approach-to-land stall, follow the procedure below:

- Configure the plane for slow flight:
    - Power to 1500
    - Sequentially deploy full flaps while keeping plane level
- At 1.3Vs0, pitch down, put the crosshair 1 inch below the horizon.  and trim for a constant-rate descent at -500 feet per minute
- The power will drop. Increase power to 1500 RRPM.
- After reaching a steady-state in descent
- Pull power to idel
- Gently pitch up into the stall
- While steering right with the rudder
- Recover the same as a regular power-off stall:
	- Relax backpressure gently
	- Apply full power 
	- Flaps to 20
	- Look for VSI reversal
	- Flaps to 10
	- Climb to a safe altitude
	- Flaps to 0
	- Pitch for level, resume level flight.

A turning stall is just adding a turn into a normal power-off (or power on) stall:

- Configure plane as desired (with flaps if power-off without flaps if power-on)
- At 1.3Vs0:
    - Bank/Ball to turn in desired direction
    - Power to idle
    - Begin to pitch up
        - The plane has a tendency to overbank at high attitudes when pulling up and turning. Opposite aileron will be needed.
    - Hold turn with rudder. Continue to gently pull the plane up unil the stall happens.

To recover:

- Relax backpressure
- Full power
- Roll level and pitch level
- Flaps to 20
- VSI reversal
- Flaps to 10
- Climb


### Flight

Today's flight went really well overall. It started off a bit rough, but once I settled in, most of the maneuvers went pretty well. Andrew is slowly allowing me to take responsibility for more things during the flight. For example, I'm starting to take on some of the radio communication. Additionally, I did the whole preflight myself, with Andrew watching to make sure I did okay.

We had a little bit of a frenetic departure. As we were doing the engine start checklist, a plane needed to taxi exactly to where we were, and we were in their way. Andrew took over to get us out of the way before we finished the checklists. Additionally, while we were doing our run-up we noticed there were several planes landing and taking off ahead of us. We did a left-downwind departure towards San Martin, in a relatively windy and bumpy bit of air. We headed south, staying below SFO's Class B airspace and SJC's Class C airspace. Andrew pointed out that normally on the downwind leg of the departure, after the crosswind leg, we like to slow down and fly level, in order to give ourselves a minute to think while we deal with norcal on the radio. Today, PAO asked us to turn right 20 degrees to get out of their way. 

We spent a lot of our flight doing clearing turns, slow flight, stalls, and steep turns. Overall, I am showing improvement. I did an especially good job of pitching for level based on the outside environment, and on trimming the plane. I still have a tendency to refer to the insturments more than I should, and I need to remember that my eyes tell me what is happening now, while the instruments tell me what the plane was doing 500 feet ago. I also still have a tendency to overcontrol the plane, though I did better at that today, especially during turbulence.

My steep turns are improving. During the actual turns, I am doing a much better job of staying level, and keeping the bank angles right. We practiced six or eight steep turns, some of which were pretty circular, and some of which were more egg-shaped. I tended to gain or lose a lot of altitude at the end of the turn, during the roll-out. It's good that I am better at holding altitude constant during the turns, but I need to avoid busting maneuvers on the roll-out.

Next, we spent about 25 minutes in slow flight. We practiced slow flight for a while, and worked on turning, climbing, descending, and otherwise operating the airplane in slow flight. The horizon was difficult to find at times, and we talked about how in the absence of a horizon, during slow flight, we should pitch for 50 knots, which is just above stall speed of 305RS. I was being too hands-on with the plane throughout slow-flight. When Andrew flies the plane, he makes sure the plane is in trim, and then uses extremely small inputs on the controls. I have a tendency to squeeze the yoke and not let go. 

Next, we moved on to the stalls. My straight-ahead power-off stalls are improving. I need to get better at memorizing the entry. At times, I deployed the flaps either early or late. Having the procedure better memorized will help me not do that. We want all of the flaps to be deployed by 1.3VS0. The flaps need to be deployed sequentially, using the plane's response as a trigger to deploy the next step. I am getting significantly better at the actual stall itself. The pull-up is more stable and gentle. The recovery is also improving, but I need to apply a lot more right rudder during the recovery. During the approach-to-land stall, I am not pulling the power all the way to idle promptly enough when it's time. Before that though, I need to make sure the power stays at 1500 RPM, so that the plane has the proper pitch. The approach to land configuration is as follows: 65 kts airspeed, full flaps, power at 1500, pitch 1 inch below the horizon. During the turning stalls, I did pretty well. I was a little bit shy about pulling in the stall, and I tended to overcontrol the plane a bit.

Finally, we moved on to ground reference maneuvers. There was a lot of wind and not a ton of visibility, so they were a litle bit difficult. I need to pay more attention to both the pylon and the horizon, to avoid gaining or losing altitude during the maneuver. I also need to have a lighter touch with the controls, even for maneuvers in which there is constant change in input. We also worked on S-turns, which are similar to turns around a point, but are more difficult and frenetic, as there is a very narrow time window for choosing a pylon. I should always hit the reference line perpindicular to it, unless the wind is at a diagonal. I was tending to overcontrol the pitch, and overbank on the upwind leg of the maneuvers. On our way back to PAO, we finished up by practicing the EGT leaning technique.


## Ground Instruction, Session 2: October 8, 2020

Today, we covered chapter 3B and chapter 2B. Fewer chapters than last week, but they were also more detailed and covered more complex topics.

### Chapter 3B

Chapter 3B covers staibility. This chapter was basically just a review of one of my mechanics courses, but with more qualatative and less quantitative analysis. The first topic we covered was dynamic vs static stability. Static stability is the tendency of a plane to return to a previous equilibrium attitude, while dynamic stability is the tendency to oscillate about that attitude before returning to it. Positive stability refers to the tendency to move towards a previous attitude, and negative stability refers to the tendency to move away from such a previous attitude. “Normal” planes are designed to have positive stability. This is nice for students, because a minor sudden movement of the control stick or a gust of wind will simply result in the plane oscillating back towards its previous attitude. Aerobatic and fighter planes may be designed to have negative stability, and will in fact “want” to turn away from straight and level flight. This is analogous to how performance cars can be tuned to be “ready” to make aggressive turns through alignment decisions.

Maneuverability and controllability are also not the same thing. Maneuverability relates to the way a plane can a) perform maneuvers easily, and b) how the airframe can respond to the stress those maneuvers place on them. Many design choices of an airplane can affect a plane’s maneuverability including size, weight, control system, and structural strength. For example, a Cessna will be much more maneuverable than a 747. Controllability, on the other hand, is how quickly an airplane will respond to a pilot’s control inputs. Stability, controllability, and maneuverability all have impact on the plane’s flight characteristics. 

The three axes of flight (us physicists would just call them i, j, and k, or maybe x, y, and z) are referred to by the following names: the longitudinal axis, which runs from front to back of the plane, the lateral axis, which parallels the wings, and the vertical axis, which goes through the plane’s center of gravity from top to bottom. Each axis has a related control surface used to rotate the plane about it. Ailerons rotate the plane about the longitudinal axis (called bank or roll), the elevators rotate the plane about its lateral axis (called bank), and the rudder rotates the plane about its vertical axis (called yaw). All of these movements are caused by a lift force. Ailerons create a difference in lift between one wing and the other, which leads the plane to roll. The elevator can create lift or downforce at the back of the plane to rotate the plane up and down, and the rudder creates a lift force to the left or right to yaw the plane. Another important thing to consider is that prop and wing downwash are designed to energize the elevator and increase pilot's control over the pitch of their plane.

Next, we talked about three rotational kinds of stability. First, is longitudinal stability, also known as pitch stability. As the name suggests, pitch stability is stability about the lateral axis, which has to do with tendencies in pitch. An important part of pitch stability is balance. The position of the plane’s center of gravity and center of pressure (or center of lift) has a lot to do with stability. Planes have a permitted “envelope” of weight and balance, which has to do with the location of the center of gravity which is permissible. In theory, if the center of gravity was exactly above (or below) the center of lift, there would be no moment induced by the difference, and the plane would fly in equilibrium with no horizontal stabilizer. In the real world, where the loading characteristics of the plane affect the location of the center of gravity, the vertical stabilizer actually creates downforce to counter the effect of torque created by the center of lift being behind the center of gravity. If the plane is loaded or if the center of gravity otherwise moves, the pilot can correct for this with trim. Being properly trimmed is in fact the result of setting tail downforce or lift to counteract the torque induced by the difference in the position of the center of gravity and the center of lift.  If the center of lift is too far forward, the plane will feel nose heavy and unstable. It may become impossible to control the plane with elevators. If the center of gravity is too far aft, the plain will be tail heavy, and it may become impossible to move the nose down in the case of a stall. Finally, another thing that affects staibility in the pitch direction is power. An increase of power will always increase stability.

Up next is lateral stability. Stability about the longitudinal axis is called lateral stability. Positive lateral stability means that a plane will return to its original attitude after a roll is initiated. Dihedral, sweepback, and keel effect have influence over lateral stability. Dihedral refers to the angle from the root of the wing to the tip. Dihedral creates a difference of lift in the direction against the induced roll. Consider a plane entering an uncoordinated roll from a gust of wind. The difference of angle of attack created by the dihedral will cause the outside wing to create less lift than the inside wing, which will cause the plane to roll back level. Low wing planes tend to need more dihedral than high wing planes. This is because with a high-wing plane, the fuselage forces air over the top of the wing, and makes it create more lift. With a low wing plane, the fuselage forces air below the wings and does not create extra lift. Sweepback, which exists in high-performance planes, will also add lateral stability. When a plane turns away from relative wind, the inside wing will have more surface perpendicular to the relative wind, and therefore will create more lift, which will result in rotation back towards its previous attitude. The keel effect, which behaves nearly the same as a boat’s keel, also creates lateral stability. As a plane rolls, relative wind creates a side force, which pushes a plane back into its previous level of roll.

Finally, and most simply, is directional stability, or yaw stability. Essentially, yaw stability is built into the plane. There is very little a pilot can do to affect yaw stability. Due to factors covered later in the chapter, light aircraft tend to have a left-turning tendency. The reason pilots are taught to keep their foot on the right rudder rather than building more rightward force into the plane is that additional rightward force would make it impossible to make a coordinated right turn in normal flight conditions. When we talked about this, we took a brief aside to the world of twin-engine light aircraft, which are incredibly directionally stable.

Next, we talked about stalls and stall awareness. As previously discussed, stalls occur whenever a plane’s wings exceed the critical angle of attack. There are two types of stalls, with some variations. Those two types of stalls are power-on and power-off stalls. The variations we discussed are turning stalls, accelerated stalls, cross-control stalls, aggravated stalls, and spins. Power off stalls occur with the power set to idle and the flaps deployed. They are close to the kinds of stalls that normally occur around the time of landing. Power on stalls are similar but occur with the engine on, similar to how take-offs are configured. We talked about stall recognition. The ways you start to notice a stall include hearing a rushing air, a buffeting of the airplane, a difficulty of controlling the plane, and noticing that much more input is required on the control surfaces. A cross-control stall occurs when a pilot has to apply excessive rudder for some reason, and then overcorrects with ailerons. The nose drops and the inside wing stalls. The airplane rolls because of the lift differential. We talked about stall recovery and important factors to consider in order to avoid a secondary stall. As a reminder, to recover from a stall, release backpressure on the control stick, apply full power, retract flaps to 20 degrees. Then look for reversal in the VSI, which indicates that the plane is leveling off. After that, move the flaps to 10 degrees, and begin to climb. After the climb is complete, retract the flaps fully and pull the power back to cruise or approach-level power. Finally, we talked about spins. We talked about how  a spin is entered when the roll and yaw are opposite of each other. For example, if you roll left and yaw right to the point of a stall, a spin could be triggered. A spin is a downward autorotation. If the plane is skidding when entering the spin, it will stay upright and if it is slipping when it enters a spin, it will become inverted. An added complication of inverted spins is that control inputs must be reversed in them. To recover from a spin, follow the acronym TARERE (terror):
```
Throttle to idle
Aileron neutral
Rudder opposite of the spin direction
Elevator nose down
Rudder neutral
Pitch up GENTLY to avoid ripping the wings off the plane
```
Finally, we talked about the flat spin, which is frequently fatal. Essentially in a flat spin, the elevator loses control of the plane after getting stuck even with the wings and the pilot is unable to recover.
 
## Chapter 2B

Chapter 2B is all about the powerplant and how it works. I will keep this summary briefer.

Airplane piston engines operate the same as car engines. They have the same four stroke cycle: intake, compression, power, exhaust. The cycle is started with an electric motor and is kept going by the cylinder timing as well as inertia in the moving parts of the engines. Airplane engines have aluminum blocks (crankcases really) and steel cylinders with aluminum heads. The heads are threaded and attached with torque and glue. The cylinders are threaded and attached to the block, rather than being integral to the block.

Turbine engines have four similar cycles, except instead of the cycles being stratified in time, they are stratified through space. Air is drawn in at the front, compressed, accelerated with fuel, and blown out the back. Power from the combustion step is used to turn the intake fans to keep the cycle going. 

In a plane with a constant speed, variable pitch propeller, a knob controls propeller pitch and therefore engine speed, while the throttle controls power. In a plane with a fixed pitch propeller, the throttle controls power by changing engine speed. The throttle controls the amount of air and fuel that goes into the engine, while the mixture knob controls how rich/lean the mixture is. Andrew likes an analogy to the water system. The mixture controls the water from the city, entering the house, while the throttle controls the tap, and modulates the amount of power that is used, as opposed to the amount of power which is available. We then talked about carburetors for a bit, and how the Venturi inside a carburetor uses the Bernoulli effect to draw fuel up into the engine. The throttle actuates the butterfly valve at the top of the carburetor, controlling the amount of fuel-air mixture entering the engine. Carburettors can ice up in surprising conditions. Because of the Venturi effect, the drop in pressure and associated drop in temperature can cause water to condense inside the carburetor and freeze, which stops fuel flow and can halt the engine. It is possible to use exhaust air to heat the carburetor. 

Many planes, including almost all of the ones I will be flying, are fuel-injected. Fuel injected airplanes, much like fuel injected cars, have pumps which spray fuel either directly into the cylinders (direct injection) or through a port (port injection). In cars, there are also common rail injection systems, especially for Diesel engines. In planes, these are not common. Most planes I will be flying will be port injected. We talked about turbochargers and superchargers, which use forced induction powered either by exhaust gases or by the engine, to shove more air-fuel mixture into the engine and therefore generate more power. We wondered if forced-induction was invented for aviation reasons. We also talked about the downsides (turbo lag and engine penalty imposed by supercharger).

Finally, we went over some of the things that make planes different. Ignition systems in piston engine aircraft are controlled by magnetos, rather than from the battery, which is charged by an alternator, as in a car. A magneto is made up of a rotor and a stator, which includes permanent magnets. When the magnetic field alternates inside the magneto, an electro-motive force (which is actually just a voltage but shhhh) is generated, which is then routed, using timing gears, to the spark plugs at the proper times. Each cylinder has two separate spark plugs, each wired to one of two magnetos. The two systems are independent and if one fails, the other will continue to operate. We talked about abnormal combustion, namely detonation and preignition. Airplane engines cannot withstand detonation as well as car engines, and sometimes if detonation occurs,  a cylinder head can simply fly off. Normal ignition is deflagration, or burning. Finally, we talked about fuel systems. Some fuel systems, for high-wing, carbureted planes, are gravity fed. Most planes that I will be flying have both an electric fuel pump and an engine-driven one. The electric one is a back up, and is used for start-up. We also talked about the components of a fuel system: fuel tanks, tank vents and drains, fuel quantity gauges , the fuel selector valve, and the pumps and hoses. We also talked briefly about oil systems and their roles. Most planes have a wet-sump system with a lot of oil (up to 12 quarts in some cases). Oil has two important roles: lubrication and cooling. Because airplane engines are air-cooled, the oil is utilized as a coolant much more than in a car.  
 
 
## Flight 5: October 3, 2020

Today, we didn't try anything new, just practiced the things I was having the most trouble with. Those things are power-off stalls, steep turns, and slow flight. Today the air was extremely smokey and didn't have great visibility, so we held off on power-on stalls, which we need a good strong horizon to practice with. Overall, I had a great flight. I felt a lot more comfortable than I have before with the controls. I still made plenty of mistakes, as expected, but I also felt a lot more in control than last week, for example.

### Ground, Pre-Flight
Today's pre-flight was abbreviated, because Andrew ran a bit late, and we weren't doing anything new. I did create an account in IACRA and signed up to get an official student pilot certificate, which will allow me to legally solo, once it's time. I do not forsee that happening any time soon, but it's nice to get the paperwork out of the way. We did a quick weather briefing, talked about how the haze and smoke were definitely going to be a factor today, and got on our way. We flew in 305RS, which is one of the newest planes in Aviation's fleet. We noticed that it hadn't been perfectly put away. The control lock was out, light switches were in the wrong positions, and the avionics master switch was on. We cleaned up, set up for flight, and topped off the fuel. I also got my own C172 checklist and was able to carry out most of the pre-flight myself. We noticed that a new left tyre had been installed since we squawked flat spots on it last week. We also talked about airport markings. Additionally, we added to the list of pre-flight checks the proces of checking the flight and engine instruments. 

### Flight

I was able to do the start-up myself, taxi away using terminal-side taxiway Yankee, to runway 31, as is standard procedure given the winds. During the run-up, we went over more details than usual, because I asked a lot of questions. This is a good thing and a bad thing. Gaining more knowledge is always good, but also we tend to spend a lot of time on the ground, because I ask a lot of questions. A couple of times during the run-up, I let my feet come off the brakes and and we actually started rolling. I need to remember to keep the foot on the brakes, hard. We took a right-dumbarton departure, and were planning to fly over the East Bay to practice various things. 

I did the take-off myself this time, and did not feel particularly overwhelmed. I even managed to do the 10 degree noise-abaitment turn to the left, as I was trying to. I did need to ask Andrew for some help with the radio communication, but I managed to handle the climb and turn alright myself. We needed to stick below 1500ft A.G.L., as we needed to stay out of SJC's Class-C airspace. Today, because we were practicing new things, I made an extra mental note to keep an eye on altitude changes during maneuvers. 

After the take-off, we made a few large-radius turns to help orient me to the new space around the east bay. We flew over Fremont, looked at Mt.Diablo, the coyote hills, and Leslie salt. We then started the meat and potatoes of the lesson with some steep turns. Initiallty, I was a little rusty on the steep turns, but after a few, I was quickly gaining comfortability on them. Some general notes from the steep turns include the following: once, I forgot to lock the friction lock of the throttle after making a power adjustment. Because of that, when I was in the process of turning, I pulled off power inadvertently, and consequently lost some altitude. In general, my right foot is too lazy. Andrew said I need to essentially double my effort on the right foot. I have a nasty habit of pushing with my right foot and then immediately letting go, as if the job is done. I need to maintain more consistent pressure on the right rudder. Once, at the end 
of a turn, I corrected trim in the wrong direction. In general, but especially evident with steep turns, I need to be a bit more assertive with the airplane. This tendency to be overpowered by the plane showed itself during the roll-out of steep turns. I need to pitch down more aggressively at the end of them to avoid gaining altitude.

After many steep turns, we moved on to practicing slow-flight. I was significantly more autonomous about slow-flight today. I had questions about how to know when the right time to deploy more flaps is, and the answer is essentially "when it feels like you need to, based on relief of control pressure". I am getting better at building a sense of when the stall horn starts to kick in. I need to do better at keeping my hand on the throttle when it's not doing other things (a common theme). I need to also use a lot more right rudder during slow flight, accompanied by opposite aileron. I also learned to do better about adding power and then pitching the plane down during slow turns, in order to keep the stall horn off.

After slow-flight, we practiced the power-off stall a few times. My entry was mostly okay. I did a good job of pulling up, and my tendency to keep the plane straight with opposite aileron is good. I need to get better at pulling up woth the proper posture, straight and square to the yoke. During the recovery, I had a tendency to dive the plane. In order to end the stall, all I need to do is leave off of the backpressure a tiny bit just to drop the nose. At the beginning of our practice, I was tending to push the yoke too hard. After a few tries, I got better at just relaxing the pressure a bit. I always need to move to full power during stall recovery. A few times, I moved to half or 3/4 power, and then moved on to do other things. This is an overreaction to last week's habit of slamming the throttle in too fast. It's okay to take 3-5 seconds to push in to full power, but I always need to go to full power in the recovery of stalls. 

Before we moved on to ground-reference maneuvers (which we only did briefly, as the sun was going down), we talked about how important it is to keep power-levels in mind always. We talked about how you may change the power, then otherwise change configuration of the plane (by deploying flaps for example), and then the power setting would change again. Additionally, when reducing power, as the airflow slows down around the plane, the power will drop again. I frequently found myself reducing power to 2000 RPM, and then needing to bump the power back up 150 RPM or so after a few seconds. This is called "babysitting the throttle". Finally, we practiced some turns around a point. I found myself paying too much attention to the GPS ground-speed indicator. I also found myself drifting inside of the proper location during the upwind section of the maneuver. That is apparently the hardest part of the maneuver. 


## Ground Instruction, Session 1: October 1, 2020

Today, I had my first ground-instruction session. In ground instruction, I will learn more about things like the physics of flight, necessary meteorological knowlege, flight planning and decision making, and other necessary things that are not directly related to flying. For our ground instruction, I am using the Jeppesen's Privot Pilot's Manual (aviators really like to call books "Manuals"). Today, we covered chapters 1, 2, and 3. There were several things that I thought I would know, that it turned out I did not.

### Chapter 1

#### Section A
Section A covers some basic background, mostly things that I already know. Because of this, my entry about it will be rather short. We covered things like how long class III medical certificates last (which is 5 years, counted by calendar months, not counted by calendar days. This means you can effectively get a free month by getting your certificate on the first of the month). We also talked about the two most important what it means to be the pilot in command of an aircraft Additionally, we covered airplane class and category. Category refers to the overall type of the aircraft: "Airplane" is a category, as is "lighter-than air", "rotorcraft", and so on. "Class" refers to a more specific type. For example, "Single-engine, Land" is the kind of aircraft I am learning to fly right now. There are also "Single-engine, Sea", "Multi-engine, Land", and "Multi-engine, Sea" airplanes, as well as gliders. Finally, we spoke about logbooks and how while the only legally requrired logbook entries are for training and currency, it is a very good idea to keep rigorous logbooks.

#### Section B

Section B is titled "Aviation Opportunities," and there are only a couple of useful pieces of information in it. We talked about airplane cagetories based on plane load limits, which include normal, utility, aerobatic, and so on. We talked about where in a pilot's operating handbook this information all lives. We also talked about a couple of groups (notably the Aircraft Owners and Pilots Association). Finally, we talked about various ratings and endorsements which I could get, once I have a pilot's certificate. These include a tailwheel endorsement, an instrument or MEI rating, a seaplane rating, or a high-performance or complex endorsement. We also talked about type ratings, which apply to planes with a weight of over 12.5 thousand pounds, or which use jet fuel, or which have turbine engines. 

#### Section C

Section B covers an introduction to human factors. During this section, we talked about a number of things, most of which can fit either into the category of Aeronautical Decision Making and Pilot In Command Responsibility. We talked about how A.D.M. includes things like making good decisions about whether to make a flight or not, given weather conditions, whether to make maneuvers we paln to, and other decisions in or related to airplanes. We talked about Single-Pilot and Crew Resource Management. We talked about how it's important that a pilot learns to do everything inside an airplane, in order to make sure that they are able to manage a flight themself. We also talked about the accident chain. Consider an example: Let's say I promised to be my friend's best man in his wedding tomorrow in L.A. I wake up the morning of after a late night out. Initially, I had hoped to leave early in the morning, but I got sidetracked with errands and work. By the time I make it to the airport, I'm already running late. I abbreviate my pre-flight and fail to check my fuel levels. I take off into deteriorating weather conditions, because I decide I have to get to LA ASAP. Now, winds are picking up, and it's starting to rain. Clouds are rolling in. Midway through my flight I notice I'm low on fuel. Now the sun is setting, and there is a layer of clouds below me. I try to land to the minimums at a nearby airport, but the fog goes too low. I have to do a go-around while I'm having a fuel emergency. Bad things can happen in this situation. The whole thing could have been avoided if I just didn't have a long night out last night.

After that, we talked about how to manage resources. We talked about how resources can include things like charts, information on ipads, communication with ATC, other pilots, people around the club, autopilot, in-plane technology, and other things. We also talked about how situational awareness is important, and that essentially, situational awareness is about paying attention to what's going on. We compared airplane situational awareness to that when one is operating a car. We remarked about how one needs to constantly be looking at engine gauges and instruments, and paying attention to the radios, looking at the horizon, and paying attention to wind and weather conditions.

We also went over the following acronyms to understand when it is safe to fly:

```
Illness
Medication

Sleep/Stress
Alcohol
Fatigue
Eating

and

Macho
Invulnerability
Impulsivity
Resignation
Anti-authority
```

### Chapter 2

#### Airplanes

We talked about the powerplant, fuselage, and empennage. The Powerplant is the area including the engine, and goes from the propeller back to the firewall. The Fuselage is the whole area that includes the cargo compartments, passengers, and so on. The Empennage is the "tail feathers" - the stabilizers and control surfaces. We talked about monocoque and semi-monocoque designs. With a monocoque, the skin is structural, and tension in the skin is important to the structural stability of the plane. In a semi-monocoque design, the skin of the plane is reinforced with struts and "ribs" such that a dent or break in any single section of the plane does not harm the structural integrity of the plane. We talked about how flaps provide extra lift and also extra drag. They can be used to slow down the plane, as well as to allow for slow-flight by increasing the amount of lift. We also talked about how planes can fly with flaps extended at speeds higher than VFE.

We talked about landing gear, and the difference between tricycle and tailwheel, and the fact that gear is made of an alloy called "spring steel" which has a stress-strain curve that allows it to experience a lot of elastic deformation, which makes it stand up to landings better. We talked about how Cessnas do not have antilock brakes, and as such are quite easy to flat-spot tyres on.

We also talked about some abnormalities of light aircraft engines. First, they have removable cylinders, rather than a block like normal car engines. They are also almost always aircooled. They have pushrod valves, and valve timing is adjusted by changing the length of the pushrods. They also are not very efficient, because they need to burn a lot of fuel, in order to create enough torque to drag a plane through the sky. Finally, they are canted to the right, because they have left-turning tendencies. 

#### Documentation

Planes must have specific documentation. We talked about this a bit while we were waiting for fuel last Sunday, but the basic idea is as follows. Since March of 1979, the FAA has required that planes have an FAA approved Pilot's Operating Handbook (Approved Flight Manual). These manuals are certified by the FAA and must contain specific content in a specific order. Additionally, whenever equipment is added to a plane, a supplement must be added to the manual which covers it. The organization is summarized by the acronym below:
```
General
Limitations
Emergency procedures
Normal procedures

Performance

Weight and balance
Airplane and systems
Supplements
Safety
```

### Flight Physics

Relative wind is the movement of air relative to the motion of the airplane. It is measured in relation to the nose of the airplane. The important thing to learn about relative wind is that failing to think about it can lead to strange and dangerous situations. Consider the idea of a level-pitch descent. Now, the relative wind is pointing up, as well as towards the back of the plane. The angle of attack of the wings is thus higher than if the plane was in normal level flight. Therefore, it is possible to stall while pitched lower than the stall angle of the airplane. This needs to be kept in mind. Moving from there, we talked about the concept of angle of attack in general, and how lift is increased as a function of angle of attack, until the critical angle is hit and the plane stalls. We also talked about the aspect ratio of wings and their shapes, and the effects these design decisions have on the planes. 

We moved on to Lift, Drag, Thrust, and Weight. We talked about how weight (which is a vector quantity) vaires in flight with load factor. When you are at 60 degrees of bank, you are experiencing 2Gs of force, as is the rest of the airframe. The propeller energizes the tail and sends high-pressure air at the tail. This gives better control. We also talked about parasite vs indudced drag. Parasite drag, which is what a physicist would just call "drag" is related to airspeed and shape of the airplane, as well as interference from airflow off of various parts of a plane. Induced drag is not actually drag, but is instead a reductuion in lift due to wingtip vortices. The wingtip vortices pull air down behind planes, and essentially "grab" the downwash creating a reduction in lift. We also talked about how the ground-effect is not in fact a "pillow of air" but is instead an effect which occurs at heights too low for the induced drag to exist. Finally, we talked abouut the best-glide speed, which is where overall drag is the lowest. The best glide speed exists at the cross-over between parasite drag and induced drag, and will be the speed where you get the highest lift per drag ratio.

## Logbooks and Note-Taking: September 28, 2020

The FAA requires that you keep an accurate record of all the flights you take. Most pilots keep records in excess of what the FAA deems necessary. I am striving to land on this side of the coin as well. Many people, myself included, keep "official" logbooks on green ledger paper, with entries that look something like this:


![sample-logbook-entry](https://cdn.boldmethod.com/images/learn-to-fly/cfis/logbook-advice-for-every-pilot/3.jpg).

However, I usually fill out my "official" logbook only after the flight is over and the postflight inspection has been done. During the pre-flight and flight, I keep notes in a separate small notebook, which I keep on my kneeboard for easy access while doing other things. I am still working on the format, but I have attached a sample notebook page below as an example.

![inflight-notebook-page](inflight-notebook-page.jpg).

After landing, I fill out my official logbook, enter flight details into ForeFlight on the ipad (preferrably with flight track logs), and have a debrief with Andrew. I take notes pre- and post-flight in a large notebook, and those notes later become the basis of these blog posts.


## Flight 4: September 27, 2020

### Ground, Pre-flight

Went over notes from yesterday’s flight (Andrew and I were both super tired so we did a very minimal debrief last night. Filled in from notes today. This portion of today’s notes have been backported into yesterday’s entry.)

We talked about the power-off stall, why we need to do it, what we are going to do. That is summarized below:

0. Configure plane for slow flight (up to the reintroduction of power) As a reminder, here are the steps:
    1. Power to 1500
    2. Flaps to 10 degrees
    3. Pitch for level
    4. Flaps to 20
    5. Pitch for level
    6. Flaps to full
    7. Pitch for level
1. Now, pull the plane up to start to induce a stall
2. Get to 1.3Vs0, move power to idle (900 RPM)
3. Carefully pull plane up to stall attitude
	Stall attitude is whatever attitude we need to stall (depends on a ton of things)
4. May have to correct pitch with ailerons (gently)
5. At top of maneuver, we experience airflow separation. This is where we feel the stall happen
6. Airplane drops the nose. If we want to recover, we just let the nose drop, and release the backpressure. Then, we go full throttle, and climb out (will touch on recovery later)
7. If we don’t want to recover, and instead want to do the “falling leaf” maneuver, we just hold the plane at the edge of stall, and let it oscillate.
8. Now, here are the details for recovery.
9. Release backpressure and let plane nose fall
10. Promptly but smoothly go to full throttle
11. Aggressively pitch up for a climb
12. Sequentially release flaps, first to 20 degrees, then 10
13. Climb with flaps at 10 degrees.
14. Retract flaps fully when we level off, at a safe altitude.

### Pre-flight
I did most of the pre-flight inspection myself! I am starting to gain confidence with the pre-flight procedure. We spotted a bunch of flat spots on the tyres, and had to go back inside to squawk it. We also needed fuel, and were stuck at the mercy of the fuel truck for quite some time, about 45 minutes. While we waited, we talked about the operating manual, certification process, MFD and radio operation, and did a practice weight and balance calculation, on paper. Once we finally had our fuel, we started up and I taxied away to the run-up area, after asking for permission. Apparently, this is something we only do at PAO, most airports will let you go to the run up area just whenever. Today, I also remembered to hit “record” on ForeFlight before our take off, so I can look at the flight log to evaluate my performance afterwards. The ForeFlight log stopped recording in the middle of the flight, so i have about 2/3rds of the history It’s available here (https://www.foreflight.com/s/track/1601237172-5DEBE476-64C3-4EA0-AF06-0E38C6741518/). We waited in the run-up area for another half an hour or so. There was a whole lot of traffic coming in and out of KPAO, and we had to wait for both.

### In-Flight
 After about 0.5 hobbs-hours of time, we finally got clearance for take-off. Andrew helped me out because we wanted to go fast to allow traffic behind us to continue what they were doing. We took off with a left-dumbarton departure and climbed to 2500 ft, before heading north towards half-moon bay. On the way out there, we got a bit of turbulence coming off the mountains, and requested permission into climb above it. We received said permission and climbed up into a layer of smoke and haze, but no turbulence. Up there, we practiced steep turns, slow flight, and power-out stalls. Power off stalls were a bit scary the first time, but honestly kind of fun. After that, we had to book it back to PAO because the plane had a reservation right after ours. Did a quick landing, taxi and postflight. 

### Post-flight debrief:

If I could only choose one thing from this post-flight, it would have to be “keep your damn hand on the throttle.” I absolutely need to keep the hand on the throttle, especially during maneuvers which require throttle changes throughout. Even when I don’t do such maneuvers, though, I still need to keep the hand there so that I can change the power setting without delay when I need to do so. 

I also need to get better at dealing with turbulence. I am not used to experiencing turbulence in a light aircraft and so I need to be better at just trusting the airplane. Essentially, we were getting non-laminar wind off of the mountains, and it was shaking the plane a bit. Nothing to worry about, but it felt like we were shaking. 

When I do steep turns, I need to be more prompt with the throttle and more precise with trim, so that I can un-trim the plane when I’m done with the maneuver. Also, in the midst of turns, I should not look at the gauges. I should be looking at the horizon, and paying attention to where I’m going. Additionally, I don’t need to look at the throttle, just move it in an inch. Additionally, when I’m in the turn, I need to keep my head in the same place rather than moving over to the left or right. Moving changes my frame of view, and I lose reference to the horizon. This results in inadvertent climbs or dives. At one point I was climbing 300 feet through the course of a 360 degree turn. That’s not ideal (or permissible).

I’m also hesitant to go to the full 45 degrees of bank. I just need to do it when I want to. The crosshair needs to stay in the right place along the horizon. I can also use the glare-shield to measure the angle rather than anything else, because it is close to the windshield and allows me to see outside too. Another thing to remember is that if I screw up a maneuver, I should just stop the maneuver, recalibrate, and try again. 

From today’s slow flight, I need to be better about keeping the crosshair at or above the horizon. I waited too long to deploy flaps. I need to be more prompt about both 10 degree flaps, 20 degree flaps, and full flaps. They all have to be done by the time i hit 1.3Vs0, which is about 65 kts in a C172. I also have to do more right-rudder all the time in slow flight. When the plane weather-vanes with the wind in slow-flight, I correct with opposite-aileron. When turning in slow flight, I need to put the nose down to keep airspeed and add power to keep altitude. That is understandable because slow-flight is in the reverse-command region, so power is controlled by altitude while airspeed is controlled by pitch. Additionally, I should bank as shallow as possible, then add power, and bank more after power is added.

In general, I also need to be smoother with the throttle. In turns, I shouldn't come off of the rudder until the turn is complete. In the power-off stall, I need to be better about putting the mark on the horizon before being ready to stall. Today, because of the haze, the horizon wasn’t clear. I will build intuition about that. Additionally, I need to remember to take the flaps off after level-off, and it’s okay to climb with 10 degrees of flaps deployed. 

Final overall notes: I have a tendency to over-control the airplane. I need to let the plane fly through gusts and turbulence. Andrew likened it to a car going over a speed bump. If you steer the car while going over the bump, you make the bumping tendencies worse. Also, I look at the instruments too much. I need to focus more on the plane and the horizon. 


## Flight 3: September 26, 2020

### GROUND: 
Went over notes, mostly. Talked about takeoffs, steep turns, more on ground reference maneuvers. Talked about specific takeoffs at PAO - gotta go 10 deg to the right, noise abatement reasons.

Main departures: Left-downwind (make a 180 after t.o.), Left dumbarton (make left and follow bridge (after going tendeg right)), right dumbarton (same thing but make a right turn)

Approaches, basically they will tell us what to do. Either NorCal or PAO.


### AIR:
We took a left-downwind departure, towards San Martin. Flew over to san martin at ~1500 feet, rising to 2500. Take-off was a bit rough. I wasn’t so good with the throttle, especially. Also, need to remember to use the friction lock. After takeoff, we flew through SJC’s airspace around to san martin. On the way there, we practiced slow flight a couple of times, and the recovery.

After we got there, we practiced rectangular course, did a touch and go, and finally took off again followed by some ground reference maneuvers. Did a whole bunch of circles, a couple of s-turns. Was quite a gusty day. Winds ~25 kts with gusts in odd directions. Part of that is that it was afternoon. 

Had a lot of trouble finding the right trim today. Not super sure why. Additionally, I felt that i was a bit worse than last week on holding level through maneuvers.

After that, we practiced some steep turns (where there’s a lot going on.) We also practived slow flight again, before really booking it back as the sun was going down. Went over moffet field (whhere we noticed that radio was cutting in and out.) Eventually, moffet handed us off. Noted that KPAO tower was already closed, so we would be landing as if it was a non-towered airport. Did so, with some minor confusion. Moffet told us there was traffic. We did a left-360 to let them go by, moffet informed us they were. at 600 feet and on final. On our approach, we didn’t see anyone. Noticed that there was another plane who was taxiing away from runway. After landing, we saw another plane land just behind us. He had to do a go-around due to the plane we had seen taxiing away.  Little bit of a near miss not helped by the fact that not very much was coming through on the radio.

### Ground, Post-Flight (Backported from tomorrow):

Today’s headset was really irritating. Mic kept flying away from my face so Andrew couldn’t hear me. Additionally, volume was imbalanced and louder in the left ear. Headset had only one volume knob. 

Andrew and I had both noted that the plane was pushing me around all the time. I need to be a little more assertive with the plane at times. Especially on pitch, I need to really tell the plane what I want it to do. I’m definitely not going to break the plane, and I’m not going to drop it out of the sky. Plus, Andrew won’t let me get even close to that.

Additionally, I need to start to internalize the phrase “Aviate, Navigate, Communicate (in that order)”. During take off (which was my first take off) I was a little too concerned with what ATC was saying and not focusing enough on flying the darn plane. 

Another few small notes. Power changes need to be more prompt, and I need to get better about what “without delay” means. When making turns, I need to choose landmarks which are further away from me. That way, I will have a better frame of reference for what a turn’s arc-length is.

I practiced slow-flight a few times, and need to think about some things. The airplane tended to overpower me during slow flight. I noticed I need to use a whole lot more control surface in slow flight, especially right rudder. I also need to be much more aggressive about pitching for level flight, and how that’s different in slow-flight. Also, when I turn, especially in slow flight, I need to be more aggressive about pitching the plane to not gain or lose altitude. 

In general, the deeper the rudder, the more I need to put on opposite aileron to deal with airplane’s overbanking tendencies. In turns, sometimes, especially in slow-flight, I need to add power to maintain altitude. I also need to remember how the reverse-command region works, and how to control altitude with power and airspeed with pitch.

In slow flight recovery, I need to do a couple of things better. First of all, I need to apply flaps more precisely. Additionally, I tend to drop my hand off the throttle. My nhand needs to live on the throttle. I also add too much friction on the friction lock. It needs to be ¼ turn away at all times, so i can quickly react to the need for more or less power.

Today’s turns around a point and steep turns went much better. I am starting to gain proficiency in turns around a point, correcting for wind.


## Flight 2: September 19, 2020

### GROUND (Theory): 
Today, we mostly covered ground-reference maneuvers, and we also worked a bit on steep turns. 

#### Procedure for steep turns:

1. Clearing Turns, to make sure you’re clear of people, 1500 ft A.G.L, ID a landmark, establish approached level (90kts @2100rpm in a C172S)
2. Bank/ball to 30 deg, maintain crosshair
3. Upon passing 30 deg bank, pitch up, to maintain crosshair.
4. Throttle in 1 inch
5. Trim, one full half turn nose up (wheel goes from top to bottom ONCE)
6. Maintain crosshair through turn. Hold rudder in direction of turn. Neutral/opposite bank depending on wid.
7. To recover, Bank/Ball, Pitch, Power, Trim. Bank/ball opposite to roll in.

#### Ground-reference maneuvers (turns around a point, S-turn, rectangular track)

##### Turn around a point:

1. Clearing turns, 600-1000 feet agl
2. Enter perpendicular to pylon, ⅛ mi away. Go abeam downwind.
3. Adjust bank angle consistent with groundspeed ot maintain constant radius around pylon.
4. Use landmarks at each 1/4 turn to adjust bank angle
5. Articulate out loud required bank angle.

When DOWNWIND, W/TAILWIND, you are going FAST and need a STEEP bank angle
In CROSSWIND situations, you may need to CRAB. MEDIUM bank angle
In UPWIND conditions, HEADWIND, you are SLOW and need a SHALLOW bank angle.

##### S-Turn: 

Essentially two HALF turns around a point in different directions. First, Identify common reference line (roads are good) around which to fly two half turns. While on the line, choose landmarks to be your pylons

The actual steps are the same as for turning around a point.

##### Rectangular course:

A rectangular course is four quarter turns around a point, connected with segments between each corner. They create a rectangular course. The rectangular course is the same as the departure procedure as well as the approach for a landing. 
 
The actual steps are the same as for turning around a point. Additionally, with cross-winds, during legs, we need to crab into the wind to avoid drifting off course. This is true in the turns around an S and point, but there is more room to drift off, when we are going straight longer.

### PREFLIGHT:
Always keep official logbook AND backup notebook. In backup notebook, we can keep logbook info, plus notes, and also things ATC tells us in the air. Pre-flight notebook info:

Header at top of page, description of flight aand what we’re doing this time around. Then, top right corner: date & tail number.

- T.F.Rs: Use the website for short &/or local flights. Use phone call for XC planning.
- T.A.F: Write down relevant weather. Example:

    ```
    FROM SJC as of 1730Z
	  FM 220Z 301/11kt v6+ Few 2k
    ```
    
- AND METAR, but don’t need to write bc we will get data from ATIS before flying.
- Track start, end tach and hobbs time. Engine start, wheels Up, wheels Down, engine stop.

Example ATIS entry: 

```
PAO -I (Measurement location & time [alphabet letter for hour of day]). 2347Z
320/11
10SM vis
CLR skies
29.90 InHg
31 (density ?)
```

- Check NOTAMs for places you’re going. ATC will yell at you if you’re breaking the rules.

- To request taxi:

```
Palo Alto Ground, Cessna TAIL # at advantage, ready for taxi. With Indigo for a Left-downwind departure towards San Martin.
```
There are also other types of departures and so-on. Additionally, this request permission for taxi is PAO specific. We don't do that at other airports.

### IN FLIGHT / Debrief:

Planned to make a downwind departure left off the runway towards San Martin, where we would practice ground-reference maneuvers and possibly a touch and go landing. We did exactly that.

Today was about airmanship. Practicing turns, climbs, descents, etc. Not a lot of maneuvers where we have to configure the aircraft. A ton of trimming to make the airplane work with me. Today I learned a whole lot about how sensitive the aircraft is (especially w.r.t trim and pitch.). 

Overall notes:

- Be better about checking crosshair on the horizon
- The horizon is top of farthest visible mountain, if possible
- HOLD YOKE AND FEEL PRESSURE BEFORE TRIM.
- DO NOT fly plane with trim wheel
- Know where the horizon is.
- Think about L/R, Slip/Skid.
- During turns, pay attention to attitude.
- Having roads to follow is helpful, like flying over graph paper
- On circles & S-turns, I was too steep i the medium->shallow upwind sector. Overall I did rather well with circles and rectangles.
- Pitch change turing a turn changes ground speed, this messes everything up.
- On the way back i practiced slow flight ad did the descent into the landing.


## Flight 1: September 8, 2020

NOTE: this flight entry was made well after the flight occurred, so the formatting won't be perfect by any means.

### GROUND

Before flying:

- Restricted zones
- NOTAM & weather
- Check out plane

LOGBOOK ENTRY:
Logbook entry must contain: 

- Name
- Tail number
- Date/time (Zulu[UTC] and Local)
- Weather briefing (more info later)
- Hobbs time - start
- Tach time - start
- (fill in others, once you land)
- Time up and time down

### AIR / Theory:

#### Maneuvers:

##### Climb:

1. Pitch (Up, a bit above horizon)
2. Power (increase)
3. Trim (to release controle stick pressure)

##### Turns:

###### LEFT:

1. Bank  (aileron)
2. Rudder (not necessary for left)
3. PITCH constantly
4. Trim (if nec.) for long turns
5. Out with RIGHT RUDDER

###### RIGHT:

1. Ball (Left rudder)
2. Make sure not overbanking (60 deg feels like wheeeee)
3. Pitch constantly
4. OUT with AILERON and then RUDDER

##### DESCENT:

1. Opposite of CLIMB but more complicated. It's more complex beacause climbing is power-limited. Can descend in many ways.


### NOTES:

- Ground-level (taxi): Tend to go right due to extra braking on Right. Focus on extra left-side braking
- More right rudder, in general. THe plane really wants to go to the left.
- For left turns: aileron in, out with right rudder pedal. For right turns, in with rudder, out with aileron + rudder (in that order)
- Do better at keeping plane level through turns. Through a turn, continually check crosshair against horizon
