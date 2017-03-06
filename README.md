# SignalCrashFucker

CFRunLoopRef runloop = CFRunLoopGetCurrent();
NSArray * allModels = CFBragingRelease(CFRunLoopCopyAllModes(runloop));
while(1){
  for(NSString * mode in allModels){
    CFRunLoopRunInModes((CFStringRef)mode, 0.001, false);
  }
}
