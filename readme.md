xcodebuild -project Unity-iPhone.xcodeproj \
  -scheme Unity-iPhone \
  -configuration Release \
  -archivePath build/UnityApp.xcarchive \
  CODE_SIGN_IDENTITY="" \
  CODE_SIGNING_REQUIRED=NO \
  CODE_SIGNING_ALLOWED=NO \
  archive


  xcodebuild -exportArchive \
  -archivePath build/UnityApp.xcarchive \
  -exportOptionsPlist ExportOptions.plist \
  -exportPath build/ipa-output
