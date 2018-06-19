# PackageApplication
PackageApplication is still here waiting for you, even if Xcode 8.3.2 excluded it, so what ?   

## Usage
Copy `PackageApplication` script to this directory `/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/usr/bin` , 
then you have to give it authority to this script ,like this `chmod 777 PackageApplication`

<br/>

Run the following command the application will be packing to a ipa file 
<br/>
`xcrun -sdk iphoneos PackageApplication  -v youapp.app -o $(pwd)/youapp.ipa`


## Xcode 命令行打包ipa

1.cd 进入工程目录下 有.xcodeproj文件的目录

2.xcodebuild clean

3.xcodebuild -scheme EasySchool -workspace EasyShool.xcworkspace build

4.xcrun -sdk iphoneos -v PackageApplication ./build/Release-iphoneos/EasySchool.app -o ~/Desktop/EasySchool.ipa

