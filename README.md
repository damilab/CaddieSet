# kimcaddie

This dataset contains golf swing analysis data, including video filenames, various golf metrics, and swing-related features during the swings. The data is intended for research and analysis in the field of sports science, particularly focused on golf swing mechanics.

## Dataset Description

We use a camera-based launch monitor to collect swing videos of various golfers and information on the trajectory of the ball

- **fileName**: The name of the video file capturing the golf swing.
- **view**: The perspective of the video (e.g., FACEON - Face On, DTL - Down The Line).
- **club**: The type of golf club used (e.g., W1 - Wood 1 / Driver, I7 - Iron 7, SW - Sand Wedge).
- **distance**: The total distance the ball traveled.
- **carry**: The carry distance of the ball.
- **ipDistanceOut**: The in-plane distance out.
- **topHeight**: The height of the ball at its apex.
- **ballAngle**: The launch angle of the ball.
- **directionAngle**: The direction angle of the ball.
- **spinBack**: The backspin of the ball.
- **spinSide**: The sidespin of the ball.
- **ballSpeed**: The speed of the ball.
- **faceAngle**: The left-right angle of the ball.
- **ballPathCode**: The flight type of the ball.

Afterward, using computer vision models, we automatically extract the joint information on the eight events of the golf swing sequence. Then, based on the domain knowledge of golf experts, we generate important features from the swing postures based on the joint values.

- **SHOULDER-ANGLE**: Shoulder angle relative to horizontal
- **UPPER-TILT**: Lower body to upper body ratio
- **STANCE-RATIO**: Shoulder width to stride length ratio
- **HEAD-LOC**: Movement of head relative to Address
- **SHOULDER-LOC**: Left shoulder position within the width of the stride
- **LEFT-ARM-ANGLE**: Angle formed by left shoulder, elbow, and wrist
- **RIGHT-ARM-ANGLE**: Angle formed by the right shoulder, elbow, and wrist
- **HIP-ROTATION**: Rotation degree of pelvis relative to Address
- **HIP-SHIFTED**: Movement of hip relative to Address
- **RIGHT-LEG-ANGLE**: Angle formed by right hip, knee, and ankle
- **SHOULDER-HANGING-BACK**: Relative distance between left ankle and left shoulder to stride length ratio
- **HIP-HANGING-BACK**: Relative distance between left ankle and left hip to stride length ratio
- **RIGHT-ARMPIT-ANGLE**: Angle formed by the right elbow, shoulder, and pelvis
- **WEIGHT-SHIFT**: Angle formed by a line connecting left ankle to left pelvis
- **FINISH-ANGLE**: Angle formed by a line connecting left ankle to right hip

