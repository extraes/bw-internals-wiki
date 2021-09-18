# class ControllerRig

Class that can be used to interface with the controller, by sending haptic feedback, getting button inputs, and getting finger curls straight from the source. It's worth noting that finger curls can also be gotten from an instance of StressLevelZero.Interaction.Hand via the fingerCurl field.

The primary and secondary interation buttons refer to the trigger and grip, respectively.

## Methods

- void ClearHasBeenGrabbed()
- bool GetAButton()
- bool GetAButtonDown()
- bool GetAButtonUp()
- bool GetBButton()
- bool GetBButtonDown()
- bool GetBButtonUp()
- GesturePose GetGesturePose(out float poseIntensity, bool forceUpdate = false)
- bool GetGrabbedState()
- float GetGripAxis()
- float GetGripForce()
- float GetGripVelocity()
- float GetIndexCurlAxis()
- bool GetMenuButton()
- bool GetMenuButtonDown()
- bool GetMenuButtonUp()
- float GetMiddleCurlAxis()
- float GetPinkyCurlAxis()
- bool GetPrimaryInteractionButton()
- float GetPrimaryInteractionButtonAxis()
- bool GetPrimaryInteractionButtonDown()
- bool GetPrimaryInteractionButtonUp()
- bool GetReleasedState()
- float GetRingCurlAxis()
- bool GetSecondaryInteractionButton()
- float GetSecondaryInteractionButtonAxis()
- bool GetSecondaryInteractionButtonDown()
- bool GetSecondaryInteractionButtonUp()
- bool GetSecondaryMenuButton()
- bool GetSecondaryMenuButtonDown()
- bool GetSecondaryMenuButtonUp()
- float GetThumbCurlAxis()
- bool GetThumbStick()
- Vector2 GetThumbStickAxis()
- bool GetThumbStickDown()
- bool GetThumbStickUp()
- bool GetTouchpad()
- Vector2 GetTouchpadAxis()
- bool GetTouchpadDown()
- bool GetTouchpadTouch()
- bool GetTouchpadUp()
- float GetTrackpadForce()
- void Haptic(float microFloat)
- void HapticAction(float secondsFromNow, float durationSeconds, float frequency, float amplitude)
- bool HasBeenGrabbed()
- bool IsGrabbed()
- bool IsReleased()
- void OnFixedUpdate(float secFromNow)
- void OnUpdate()
- void OnVrFixedUpdate()

## Fields

- Handedness handedness
- Transform hand
- Quaternion wristOffset
- Haptor haptor
- ControllerInfo.Type controllerType
- Haptor _haptor
- GesturePose _gesturePose
- float _nextGestureUpdateTime
- float _gesturePoseIntensity
- (ControllerRig)[/class-reference/StressLevelZero/Rig/ControllerRig.md] manager

## Enums

### GesturePose

- OpenHand
- IndexPoint
- MiddleFinger
- PeaceSign
- ThumbsUp
- ThumbsDown
- Fist