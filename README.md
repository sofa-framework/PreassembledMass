# Plugin PressambledMass.

It allows the precomputation of a mass matrix at the desired level (generally at the independent dof level) from mapped masses.
The mass matrix assembly is based on the Compliant plugin.
Warning: all independent dofs must be in its own branch (ie no child node without mapping).
Warning: it is only working for constant mappings, when the preassembled mass is constant.
The mapped masses are then destroyed, and given nodes (that were only mapping masses) can be deactivated automatically.
It is useful to finely defined a mass (image density for example), without having to propagate x,v,dx at each frame/iteration.
It could also permit to use mapped masses with an explicit integration (the mass inversion is not yet implemented).

(copy-paste from the 1st commit message)
