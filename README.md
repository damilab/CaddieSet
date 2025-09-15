# CaddieSet

Official dataset of the paper CaddieSet: A Human-Joint Feature Dataset for Golf Swing Analysis. * 📄 **Paper (arXiv):** [(https://openaccess.thecvf.com/content/CVPR2025W/CVSPORTS/html/Jung_CaddieSet_A_Golf_Swing_Dataset_with_Human_Joint_Features_and_CVPRW_2025_paper.html)](https://openaccess.thecvf.com/content/CVPR2025W/CVSPORTS/html/Jung_CaddieSet_A_Golf_Swing_Dataset_with_Human_Joint_Features_and_CVPRW_2025_paper.html)

This dataset contains golf swing analysis data, including various golf ball flight information, and swing-related features during the swings. The data is intended for research and analysis in the field of sports science, particularly focused on golf swing mechanics.

## Dataset Description

Swing videos and ball flight estimates of 8 individuals with diverse golf skills were collected using a camera-based launch monitor.
Our dataset consists of 1,757 shots, including 924 with FACEON views and 833 with DTL views.

- **View** : The perspective of the video (e.g., FACEON - Face On, DTL - Down The Line).
- **ClubType** : The type of golf club used (e.g., W1 - Wood 1 / Driver, I7 - Iron 7).
- **Distance** : The total distance the ball traveled.
- **Carry** : The carry distance of the ball.
- **LrDistanceOut** : The in-plane distance out.
- **DirectionAngle** : The direction angle of the ball.
- **SpinBack** : The backspin of the ball.
- **SpinSide** : The sidespin of the ball.
- **SpinAxis** : The axis when the ball spins.
- **BallSpeed** : The speed of the ball.
- **GolferId** : Identification of golfers.

Afterward, using computer vision models, we automatically extract the joint information on the eight events of the golf swing sequence. Then, based on the domain knowledge of golf experts, we generate important features from the swing postures based on the joint values.

- **SHOULDER-ANGLE** : Shoulder angle relative to horizontal
- **UPPER-TILT** : Lower body to upper body ratio
- **STANCE-RATIO** : Shoulder width to stride length ratio
- **HEAD-LOC** : Movement of head relative to Address
- **SHOULDER-LOC** : Left shoulder position within the width of the stride
- **LEFT-ARM-ANGLE** : Angle formed by left shoulder, elbow, and wrist
- **RIGHT-ARM-ANGLE** : Angle formed by right shoulder, elbow, and wrist
- **HIP-ROTATION** : Rotation degree of pelvis relative to Address
- **HIP-SHIFTED** : Movement of hip relative to Address
- **RIGHT-LEG-ANGLE** : Angle formed by right hip, knee, and ankle
- **SHOULDER-HANGING-BACK** : Relative distance between left ankle and left shoulder to stride length ratio
- **HIP-HANGING-BACK** : Relative distance between left ankle and left hip to stride length ratio
- **RIGHT-ARMPIT-ANGLE** : Angle formed by right elbow, shoulder, and pelvis
- **WEIGHT-SHIFT** : Angle formed by a line connecting left ankle to left pelvis
- **FINISH-ANGLE** : Angle formed by a line connecting left ankle to right hip
- **SPINE-ANGLE** : Spine angle relative to horizontal
- **LOWER-ANGLE** : Angle formed by right pelvis, knee, and ankle
- **SHOULDER-ANGLE** : Shoulder angle relative to horizontal
- **HIP-LINE** : Movement of hip relative to Address
- **HIP-ANGLE** : Rotation degree of pelvis relative to Address
- **RIGHT-DISTANCE** : Gap between right elbow and the torso
- **LEFT-LEG-ANGLE** : Angle formed by left pelvis, knee, and ankle

## Citation

If you use our dataset or find our work is relevant to your research, please cite:
```bibtex
@inproceedings{jung2025caddieset,
  title={CaddieSet: A Golf Swing Dataset with Human Joint Features and Ball Information},
  author={Jung, Seunghyeon and Hong, Seoyoung and Jeong, Jiwoo and Jeong, Seungwon and Choi, Jaerim and Kim, Hoki and Lee, Woojin},
  booktitle={Proceedings of the Computer Vision and Pattern Recognition Conference},
  pages={5988--5996},
  year={2025}
}
```
