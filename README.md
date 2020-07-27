[h1]Description[/h1]

Adds two new planetary decisions and one edict that can be accessed from the start of the game. The first decision, [i]Distribute Surplus[/i], adds a modifier to the planet that improves pop happiness, planet stability, and pop growth at the cost of increased food consumption. The pop growth modifier is determined from the planet's current biological pop size and its free housing, which results in logistic pop growth. The second decision, [i]STOP Distributing Surplus[/i], removes the modifier(s) added by Distribute Surplus, including the increased food consumption rate. Finally, there is an edict, [i]Distribute Surplus[/i], which costs nothing and applies the effects of the Distribute Surplus decision to each colonized planet and to new planets upon colonization. Individual planets can opt-out by utilizing the STOP Distributing Surplus decision.

[h1]Distribute Surplus[/h1]

The [i]Distribute Surplus[/i] decision applies a logistic growth modifier to the planet's bio pop growth and its growth from immigration. By default, Stellaris uses linear growth, which means that bio pop growth does not increase as the bio pop size does. Applying a logistic growth modifier can correct this to match more realistic population growth as well as provide a useful mechanic to trade food for growth.

The formula for logistic growth is dN/dt = r * N * (K - N) / K, where dN/dt is the logistic growth modifier, r=3 (which is mapped to 0.03), N is the bio_pops size calculated by Planetary Census, and K is the planet's carrying capacity. A planet's carrying capacity is K = ( (bio_pops) + (free_housing) ) * 1.5. Free housing is the planet's currently available housing. The coefficient, 1.5, is the overcrowding modifier. This determines the homeless population that the planet can support. By including an overgrowth modifier, a planet can grow a larger population than it can support, which triggers the games diverse mechanics to handle overcrowding. The final result is a population size that overshoots its housing capacity and then declines as a result. The overshoot and decline model is a more realistic model of population growth and interplays with Stellaris's existing mechanics rather well.

While the Distribute Surplus decision costs nothing, it increases the food consumption of organic species by 300% (minerals for Lithoids).

The effect of this decision is removed by enacting the [i]STOP Distributing Surplus[/i] decision, updated at the end of the month. [b]Distribute Surplus[/b] can be applied to all planets by enacting the Distribute Surplus edict, found on the edicts page. Toggling off the edict similarly applies the [b]STOP Distributing Surplus[/b] decision to each planet, which removes the effects of Distribute Surplus. Invididual planets can opt-out of the edict by enacting the STOP Distributing Surplus decision.

[h1]Notes[/h1]

The current biological pop size and free housing are recomputed every year (for all planets) and each time that the Distribute Surplus decision is enacted (for that planet).

To get the most out of each Distribute Surplus decision, a planet should have 1 free housing for every 3 bio pop. For example, a planet with 15 bio pop should ideally have 5 free housing. Any additional free housing increases the resulting logistic growth modifier and any less free housing decreases the logistic growth modifier. We recommend enacting the Distribute Surplus decision when 1 addition pop is needed to unlock the next building.

[h1]Compatability[/h1]

This mod only adds new files and does not alter any vanilla values or files. It should be compatible with all other mods. The mod order may need to be adjusted so that UI mods can incorporate the new decisions into the UI. Note that the Distribute Surplus decision is not visible unless the Planetary Census modifier has been applied to the planet from the Planetary Census decision.

While this mod should be compatible with other growth mods, such as stararchitec's Carrying Capacity, using this mod in combination with other growth mods can result in unintended consequences. No DLC required.

[h1]Future Work[/h1]

While balancing is needed, there is currently no additional work intended for this mod. We are bouncing around ideas for growth that can be applied Machines. However, we have not yet identified an idea that we feel is in the spirit of this species types.
