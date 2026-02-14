 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
new file mode 100644
index 0000000000000000000000000000000000000000..78309f35412f12d55a7170e82c3983965b2ee538
--- /dev/null
+++ b/README.md
@@ -0,0 +1,24 @@
+# Cookie Clicker Lite
+
+A simple browser-based cookie clicker game.
+
+## Features
+
+- Click the cookie to gain cookies.
+- Click sound effect on each click.
+- Mute / Unmute sound toggle.
+- Buy upgrades:
+  - Cursor: +1 cookie/sec
+  - Factory: +10 cookies/sec
+  - Mega Oven: +50 cookies/sec
+- In-game quick guide.
+
+## How to run
+
+Open `index.html` directly in your browser, or serve with a local web server:
+
+```bash
+python3 -m http.server 8000
+```
+
+Then visit `http://localhost:8000`.
 
EOF
)
