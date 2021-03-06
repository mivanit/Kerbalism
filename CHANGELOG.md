#CHANGELOG

0.9.9.7
  - re-added Food/Oxygen definitions temporarely to the default profile
  - changed key combination to mute/unmute messages to CTRL+N

0.9.9.6
  - the default profile now require CommunityResourcePack
  - NEW PARTS! inline food containers and radial oxygen tank by Tygoo7
  - NEW PART! geiger counter by Naazari1382
  - phased out old food and oxygen containers
  - messages can be muted and unmuted by using CTRL+M
  - moved gravity ring higher in the tech tree
  - experimental Realism profile
  - experimental TAC-LS emulation profile
  - fix: depletion estimates with meal-based rules
  - fix: probes and other parts getting supply resources in some occasions
  - fix: vessel info window doesn't show supplies depletion estimates for unmanned vessels
  - fix: corrected automatic waste capacity in pods
  - fix: correct depletion estimates at extreme timewarps
  - fix: greenhouse doesn't consume waste when there is no lighting

0.9.9.5
  BIG REFACTOR
  - can run arbitrary rules that consume a resource and accumulate a value per-kerbal
  - rules can be influenced by environment
  - existing mechanics reimplemented as a set of rules and enabled by default
  - with no rules it degenerate into a background simulation of the resources with ui
  - you can write your own rules, go check in profiles/ directory
  CRP COMPATIBILITY
  - food/oxygen properties have been changed to match CRP ones
  - food/oxygen consumption changed to more realistic rates
  - previous savegames will keep working (yay!)
  CONFIGURATION
  - settings.cfg to customize the simulation
  - choose a file in the profiles/ directory, create your own, or don't use one at all
  - signal mechanic is disabled automatically if you are using RemoteTech or AntennaRange
  - malfunction mechanic is disabled automatically if you are using DangIt
  OTHER MODS SUPPORT
  - SCANsat modules re-enable automatically when EC is back
  - support for NearFuture reactors, fission generators and radioisotope generators
  - support Planetary Base System converters
  - support for Origami antennas
  - NearFutureSpacecraft, CryoTanks and KerbalAtomics MM patches by Fraz86
  - greenhouse & scrubber modules work on arbitrary resources
  - more hooks added, go check out
  MALFUNCTIONS
  - malfunctioned components are highlighted, can be toggled on/off from the monitor ui
  - engineers can inspect parts and get an estimate of lifetime
  - use new curve for part aging
  - use new method to incentive redundancy
  - seriously lowered the malfunction rate
  - antennas will last longer
  - limit of 2 malfunctions per-component at max
  - reduced range penalty for antenna malfunctions
  - radiation don't influence malfunctions anymore
  - planner show correct malfunctions/year estimates
  MISC
  - recompiled against KSP 1.1.2
  - tech descriptions are updated automatically, no need to do that in MM patches anymore
  - improved tech description visibility
  - phased out the high-tech 1.25m food container
  - more robust depletion estimates
  - new Sensor module to add environment readings to a part
  - storm messages can be disabled per-vessel
  - storms can be turn off in settings
  - added a partlist icon in the vab and moved parts there
  BALANCE
  - lowered mass of shielding
  - reduced mass of parts in general
  - breakdown events also incur a reputation penalty
  - increased time before breakdown a bit
  - reduced frequency of storms
  - increased science value of experiments a bit
  - moved small fixed panel to basic science
  - rebalanced solar panels outputs to visually match number of panels
  BUGFIXES
  - fix: bug with multiple ModuleResourceConverters in background and active flag
  - fix: helmet state no forced on top of KIS anymore
  - fix: problems with flowState
  - fix: problems with resque kerbals on eva
  - fix: setup resources for resque missions
  - fix: kerbal climate property recover slowly to avoid exploit
  - fix: thermometer readings


0.9.9.4
  - new part! an artificial gravity hab by mehka
  - new part! small food container by Nazari1382
  - new part! a better 1.25m food container by tygoo7
  - added support for ConnectedLivingSpace
  - vessel info window
  - new 'medium' scope for antennas
  - doubled amount of EC on eva suits
  - minor changes in the EnergyTweaks
  - reduced radiation influence over malfunctions
  - MM patches for NearFutureElectrical and NearFuturePropulsion by Fraz86
  - default antenna patch by speedwaystar
  - greenhouse module can specify an emissive object for the lamps
  - fix: greenhouse module do not assume there is a shutter anymore
  - fix: monitor tooltip, this time for real
  - fix: antennas should work with contracts now
  - fix: issue with EVA prop getting created out of thin air
  - fix: curved solar panels weren't working
  - fix: kerbals don't stop eating anymore


0.9.9.3
  - technologies can be customized
  - radiation influence malfunctions
  - support for NearFutureSolar
  - moved all parts to utility menu
  - no more oxygen warnings at prelaunch
  - tweaked some EnergyTweaks values
  - MM patches in directory tweaks can now be deleted
  - fix: problem with EVA monoprop
  - fix: planner doesn't cover staging icons anymore
  - fix: monitor was visible in main menu
  - fix: monitor tooltip problems with scrubber
  - fix: problem with negative part
  - fix: bug in malfunction penality


0.9.9.2
  - added tags to parts
  - reverted to stock monoprop behavior from/to EVA temporarely


0.9.9.1
  - ported to KSP 1.1.0.1230
  - removed assumptions on technologies order
  - versioning of serialized data
  - doubled radiation life expectancy at max shielding
  - added CommunityTechTree patch courtesy of DarkonZ
  - monitor: vessels can be assigned to groups
  - monitor: can filter vessels by group
  - monitor: added time to depletion of Food & Oxygen to supply icon tooltip
  - planner: EC cost of active radiators respect enabled/disabled toggle
  - planner: EC cost of new wheels, respect motor toggle
  - hooks: scan for assembly only once
  - hooks: new function InjectKerbal()
  - bugfix: proper text clamping for vessel name in monitor
  - bugfix: release input locks even when not in flight
  - bugfix: human-readable durations weren't using earth time settings
  - bugfix: SCANsat resource scanners weren't consuming EC in background


0.9.9.0
  First public release


