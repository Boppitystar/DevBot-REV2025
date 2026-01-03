# Robot breakdown
This is a FRC robot built for the 2025-2026 development.

The robot is 18 by 18 inches, and has limelight. 

## Subsystems
### drivetrain (Swerve)
- 4 module Stock MaxSwerve
- Bot is 18 in by 18 in
- NavX2 is centred on base

Location from the centre With NWU coordinate system is as follows:

| Module CANID (drive, turn) | X distance from centre (in) | Y distance from centre (in) | Rotational offset |
| :----------------- | :-------: | :-------: | :--------: |
| Front Left (1,2)   | 7.25  | 7.25  | 1/2 $\pi   |      
| Bottom Left (3,4)  | -7.25| 7.25  | -1/2 $\pi  |
| Bottom Right (5,6) | -7.25 | -7.25 |  -pi  |
| Front Right (7,8)  | 7.25  | -7.25| 0 |

### Tracking
- Vision using limelight 3 camera (April tags)
- Field tracking using using Field2D in smartdashboard


## MVP Requirements
1. The robot drivetrain is capable of swerve movements (field and robot) [drivetrain subsystem]

2. The robot is capable of following a auto path with auto align robot [autonomous]

3. The robot is capable of getting pose from the apriltag [tracking subsystem]
    1. The robot is able to print different position based on the pose provided by the vision system [driving and vision subystem]

4. The robot is capable of auto align position to april tag using limelight in teleop 