# iTerm2 Without the TitleBar

![](https://raw.githubusercontent.com/dougblack/iTerm2/master/screenshot.png)

It's a one line change.

```
diff --git a/sources/PseudoTerminal.m b/sources/PseudoTerminal.m
index 33189ec..9e3552b 100644
--- a/sources/PseudoTerminal.m
+++ b/sources/PseudoTerminal.m
@@ -323,8 +323,7 @@ static const CGFloat kHorizontalTabBarHeight = 22;
             return NSBorderlessWindowMask;

         default:
-            return (NSTitledWindowMask |
-                    NSClosableWindowMask |
+            return (NSClosableWindowMask |
                     NSMiniaturizableWindowMask |
                     NSResizableWindowMask |
                     NSTexturedBackgroundWindowMask);
```

# # Installation

1. Open up this project in iTerm2.
2. Hit the play arrow in the top left to build and run.
3. Once the app opens, you can right click the icon in your
dock and go to Options &rarr; Show in Finder.
4. Replace your existing iTerm2 app with that one.
