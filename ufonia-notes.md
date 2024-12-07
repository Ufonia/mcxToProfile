# Ufonia Notes

If you see the error `ImportError: No module named Foundation`, you may need to run `pip install pyobjc` as described [here](https://github.com/timsutton/mcxToProfile/issues/25).

The command you need is:

``` sh
./mcxToProfile.py --plist ./mdm-samples/com.google.Chrome.extensions.ghbmnnjooekpmoecnnnilnnbdlolhkhi.plist --identifier com.ufonia.mdm.offline-docs --displayname "Ufonia Offline Docs" --removal-allowed
```

Once you've created the .mobileconfig file, you need to upload it to Jamf, and push it out to people's devices. They then need to full close and reopen Chrome for the "Make available Offline" option to not be greyed out. If the option doesn't appear at all, they probably don't have the Offline docs Chrome extension. 