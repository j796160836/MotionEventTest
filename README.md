MotionEventTest
==========
  
###Reproduce steps  
1. Run the sample.  
2. Long click with three finger,   
or touch back and forth with two finger and three finger. (press down a finger down, press down another one, release one finger and another hold steady.)
3. Exception throws.  
  
###Exception Sample  
  
    
FATAL EXCEPTION: main  
Process: com.example.cardscrolltest, PID: 5689  
java.lang.IllegalStateException: Could not find pointer '1' in reference point: At time 5516242:  pointer 0 ACTION_DOWN: (366.000000,82.000000) to be calculated against current event: At time 5516361:  pointer 1 ACTION_UP: (795.000000,100.000000).  
	at com.google.android.glass.touchpad.Utils.isWithinDistance(Utils.java:179)  
	at com.google.android.glass.touchpad.Utils.isWithinTapArea(Utils.java:145)  
	at com.google.android.glass.touchpad.OneFingerState.onEvent(OneFingerState.java:47)  
	at com.google.android.glass.touchpad.StateMachine.onEvent(StateMachine.java:100)  
	at com.google.android.glass.touchpad.GestureDetector.onMotionEvent(GestureDetector.java:283)  
	at com.example.cardscrolltest.HelloActivity.onGenericMotionEvent(HelloActivity.java:94)  
	at android.app.Activity.dispatchGenericMotionEvent(Activity.java:2501)  
	at com.example.cardscrolltest.HelloActivity.dispatchGenericMotionEvent(HelloActivity.java:85)  
	at com.android.internal.policy.impl.PhoneWindow$DecorView.dispatchGenericMotionEvent(PhoneWindow.java:2154)  
	at android.view.ViewRootImpl$ViewPostImeInputStage.processGenericMotionEvent(ViewRootImpl.java:3995)  
	at android.view.ViewRootImpl$ViewPostImeInputStage.onProcess(ViewRootImpl.java:3859)  
	at android.view.ViewRootImpl$InputStage.deliver(ViewRootImpl.java:3421)  
	at android.view.ViewRootImpl$InputStage.onDeliverToNext(ViewRootImpl.java:3471)  
	at android.view.ViewRootImpl$InputStage.forward(ViewRootImpl.java:3440)  
	at android.view.ViewRootImpl$AsyncInputStage.forward(ViewRootImpl.java:3547)  
	at android.view.ViewRootImpl$InputStage.apply(ViewRootImpl.java:3448)  
	at android.view.ViewRootImpl$AsyncInputStage.apply(ViewRootImpl.java:3604)  
	at android.view.ViewRootImpl$InputStage.deliver(ViewRootImpl.java:3421)  
	at android.view.ViewRootImpl$InputStage.onDeliverToNext(ViewRootImpl.java:3471)  
	at android.view.ViewRootImpl$InputStage.forward(ViewRootImpl.java:3440)  
	at android.view.ViewRootImpl$InputStage.apply(ViewRootImpl.java:3448)  
	at android.view.ViewRootImpl$InputStage.deliver(ViewRootImpl.java:3421)  
	at android.view.ViewRootImpl$InputStage.onDeliverToNext(ViewRootImpl.java:3471)  
	at android.view.ViewRootImpl$InputStage.forward(ViewRootImpl.java:3440)  
	at android.view.ViewRootImpl$AsyncInputStage.forward(ViewRootImpl.java:3580)  
	at android.view.ViewRootImpl$ImeInputStage.onFinishedInputEvent(ViewRootImpl.java:3740)  
	at android.view.inputmethod.InputMethodManager$PendingEvent.run(InputMethodManager.java:2010)  
	at android.view.inputmethod.InputMethodManager.invokeFinishedInputEventCallback(InputMethodManager.java:1704)  
	at android.view.inputmethod.InputMethodManager.finishedInputEvent(InputMethodManager.java:1695)  
	at android.view.inputmethod.InputMethodManager$ImeInputEventSender.onInputEventFinished(InputMethodManager.java:1987)  
	at android.view.InputEventSender.dispatchInputEventFinished(InputEventSender.java:141)  
	at android.os.MessageQueue.nativePollOnce(Native Method)  
	at android.os.MessageQueue.next(MessageQueue.java:138)  
	at android.os.Looper.loop(Looper.java:131)  
	at android.app.ActivityThread.main(ActivityThread.java:5045)  
	at java.lang.reflect.Method.invokeNative(Native Method)  
	at java.lang.reflect.Method.invoke(Method.java:515)  
	at com.android.internal.os.ZygoteInit$MethodAndArgsCaller.run(ZygoteInit.java:786)  
	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:602)  
	at dalvik.system.NativeStart.main(Native Method)  

