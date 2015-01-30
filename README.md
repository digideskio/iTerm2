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
