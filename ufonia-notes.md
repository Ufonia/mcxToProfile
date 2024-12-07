# Ufonia Notes

If you see the error `ImportError: No module named Foundation`, you may need to run `pip install pyobjc` as described [here](https://github.com/timsutton/mcxToProfile/issues/25).

The command you need is:

``` sh
./mcxToProfile.py --plist ./mdm-samples/com.google.Chrome.extensions.ghbmnnjooekpmoecnnnilnnbdlolhkhi.plist --identifier com.ufonia.mdm.offline-docs --displayname "Ufonia Offline Docs" --removal-allowed
```