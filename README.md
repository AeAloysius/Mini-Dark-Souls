# Mini-Dark-Souls
A third-person melee prototype built in Unreal Engine 5, featuring modular weapons, precise hit detection, stamina/poise systems, directional knockback with hit-stun, resettable light/heavy combo chains, 8-way rolls/backstep/guard, enemy lock-on with target switching, and an animation stack that combines Motion Matching with layered blends for smooth, natural transitions and reduced “mechanical” feel.

## Gameplay Screenshot
![screenshot](https://github.com/AeAloysius/Mini-Dark-Souls/blob/main/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202025-09-23%20201856.png)

## Player Controller & Core Systems: 
Movement, camera rotation, jumping, attacking, executions, lock-on/unlock with target switching, stamina consumption/recovery, blocking & mitigation, health.
## Combat Mechanics: 
Resettable light/heavy combo chains; running/sprint/jump attacks; hit detection via line/sphere traces with damage + hit-stun + 4-direction knockback; multi-hit dedupe and debug visualization.
## Defense & Resources: 
Block timing and success check; stamina timers and thresholds; poise thresholds triggering staggers/knockdowns.
## Mobility: 
8-way rolls and backstep; direction selection from velocity/acceleration; adaptive camera boom for readability.
## Animation Quality: 
Explored and integrated Motion Matching, blending with Layered Blend per Bone / Slots—upper-body attacks while lower-body stays on MM locomotion; IK retargeting for cross-skeleton reuse.
## Enemy AI (Behavior Tree): 
Blackboard + services for distance checks and state gating; patrol (random location / reach) → engage → approach → attack → react → die; coordinated with the player lock-on system.
## Architecture & Tuning: 
Enhanced Input mappings; data assets for weapons/segments/values; tunables for trace radius/length, lock-on selection (angle/distance/LOS), and camera offsets.
