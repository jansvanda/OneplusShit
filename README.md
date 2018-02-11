# OneplusShit

This is for Dvice Tree - 

You need to include the entire OneplusShit repo in your DT + Some Changes Needed - 

1) You need to include Overlay for Settings from here - https://github.com/SuperDroidBond/failed_one/tree/xtended/overlay/packages/apps/Settings/res/values (devicehandler_arrays.xml & devicehandler_strings.xml)

2) Added OneplusShit in device.mk - https://github.com/SuperDroidBond/failed_one/blob/xtended/device.mk#L247

This is it. You're good to go for DT Part. 

Settings Part (Inclusion of Device Features in Settings - 

Add it in Main XML - 

        <!-- Device Part -->
        <Preference
            android:key="device_part"
            android:title="@string/device_part_title"
            android:summary="@string/device_part_summary">
            <intent android:action="com.android.settings.action.EXTRA_SETTINGS"
               android:targetPackage="com.oneplus.shit"
               android:targetClass ="com.oneplus.shit.settings.ShitPanelSettings" />
        </Preference>

Also do not forgot do add respective strings required for it -

    <string name="device_part_title">Device Features</string>
    <string name="device_part_summary">Oneplus Shits</string>

Hope It will be worth the time.
