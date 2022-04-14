# IntegratedDriverDuplicateFilenames

`defaults write com.apple.dt.XCBuild EnableSwiftBuildSystemIntegration 0`
Results in clear error:
```
error: filename "Test.swift" used twice: '/Users/colton.schlosser/workspace/IntegratedDriverDuplicateFilenames/Sources/IntegratedDriverDuplicateFilenames/A/Test.swift' and '/Users/colton.schlosser/workspace/IntegratedDriverDuplicateFilenames/Sources/IntegratedDriverDuplicateFilenames/B/Test.swift'
note: filenames are used to distinguish private declarations with the same name
```

`defaults write com.apple.dt.XCBuild EnableSwiftBuildSystemIntegration 1`
Results in obtuse error:
```
error: Unexpected error in driver invocation: fatalError
```
