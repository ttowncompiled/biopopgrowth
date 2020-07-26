[h1]Description[/h1]

Adds two new planetary decisions that can be accessed from the start of the game. The first, Planetary Census, costs nothing and takes 28 days to complete. Once completed, it provides access to a secondary decision, Distribute Surplus. This decision costs more food with larger population sizes and adds a logistic growth modifier to pop growth and immigration based on the planet's pop size and current free housing.

[h1]Planetary Census[/h1]

Planetary Census is a new decision that costs nothing to use. It takes 28 days to complete. Once completed, it adds a modifier to the planet, Planetary Census. This modifier unlocks the decision, Distribute Surplus, which costs food and can significantly boost the planet's biological growth. The Planetary Census decision can be enacted each month and the resulting modifier lasts for 365 days.

The primary purpose of this decision to calculate the size of the planet's biological population, since only that population will be affected by the Distribute Surplus decision. Although the Planetary Census modifier adds no bonuses to the planet, it attaches a hidden biological population count (bio_pops) to the planet. The bio_pops value is used to determine the cost of the Distribute Surplus decision and is used to calculate the planet's expected logistic growth.

[h1]Distribute Surplus[/h1]

The Distribute Surplus decision applies a logistic growth modifier to the planet's bio pop growth and its growth from immigration. By default, Stellaris uses linear growth, which means that bio pop growth does not increase as the bio pops size does. Applying a logistic growth modifier can correct this to match more realistic population growth as well as providing a useful mechanic to trade food for growth.

The formula for logistic growth is dN/dt = r * N * (K - N) / K, where dN/dt is the logistic growth modifier, r=3 (which is mapped to 0.03), N is the bio_pops size calculated by Planetary Census, and K is the planet's carrying capacity. A planet's carrying capacity is K = ( (bio_pops) + (free_housing) ) * 1.5. Free housing is the planet's currently available housing. The coefficient, 1.5, is the overcrowding modifier. This determines the homeless population that the planet can support. By including an overgrowth modifier, a planet can grow a larger population than it can support, which triggers the games diverse mechanics to handle overcrowding. The final result is a population size that overshoots its housing capacity and then declines as a result. The overshoot and decline model is a more realistic model of population growth and interplays with Stellaris's existing mechanics rather well.

The food cost for Distribute Surplus starts at 120 food for 1-4 bio pop. It goes to 180 food at 5 bio pop and increases by 180 food for each 5th pop up to the 75th pop. If pop size decreases, so too does the cost. Although, the Planetary Census may need to be enacted once more.

[h1]Notes[/h1]

Both the cost of the decision and the logistic growth modifier are calculated using the same bio_pops value. As such, reducing the biological population to reduce the cost of the Distribute Surplus decision also results in a reduced logical growth modifier. In general, it is always best to enact the Planetary Census decision in preparation to enact the Distribute Surplus decision and not as a means to "lock-in" a good price.

To get the most out of each Distribute Surplus decision, a planet should have 1 free housing for every 3 bio pop. For example, a planet with 15 bio pop should ideally have 5 free housing. Any additional free housing increases the resulting logistic growth modifier and any less free housing decreases the logistic growth modifier. We recommend enacting the Distribute Surplus decision when 1 addition pop is needed to unlock the next building.

[h1]Compatability[/h1]

This mod only adds new files and does not alter any vanilla values or files. It should be compatible with all other mods. The mod order may need to be adjusted so that UI mods can incorporate the new decisions into the UI. Note that the Distribute Surplus decision is not visible unless the Planetary Census modifier has been applied to the planet from the Planetary Census decision.

While this mod should be compatible with other growth mods, such as stararchitec's Carrying Capacity, using this mod in combination with other growth mods can result in unintended consequences. No DLC required.

[h1]Future Work[/h1]

While balancing is needed, there is currently no additional work intended for this mod. We are bouncing around ideas for growth that can be applied to Lithoids and Machines. However, we have not yet identified an idea that we feel is in the spirit of these species types.
