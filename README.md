# react-native-multiDex
if you need set multiDex,you can read this.
Perhaps you can search some suggestion about this issue.
But,android 4.4.4 will crash.
Important！！！！
Don't write the codes in your activity.
sign:
app/build.grandle
multiDexEnabled true

compile "com.android.support:multidex:1.0.0"


AND  change your MainApplication extends MultiDexApplication

import android.support.multidex.MultiDexApplication;//add
public class MainApplication extends MultiDexApplication implements ReactApplication {
                                      //changed
}
I was used two days to  resolve this issue.
Because,search's answers is so bad........so I write it...
