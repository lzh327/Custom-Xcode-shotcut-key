# Custom-Xcode-shotcut-key
How to custom Xcode shotcut key

1: Copy '/Applications/Xcode.app/Contents/Frameworks/IDEKit.framework/Resources/IDETextKeyBindingSet.plist' to desktop.

2: Add following contents into the .plist file:

    <key>My Custom Actions</key>
    <dict>
        <key>Insert Line Below</key>
        <string>moveToEndOfLine:, insertNewline:</string>
        <key>Insert Line Above</key>
        <string>moveUp:, moveToEndOfLine:, insertNewline:</string>
    </dict>

3: Copy back the modified file.

sudo cp ~/Desktop/IDETextKeyBindingSet.plist /Applications/Xcode.app/Contents/Frameworks/IDEKit.framework/Resources/IDETextKeyBindingSet.plist

4: Restart the Xcode and perform key binding.


