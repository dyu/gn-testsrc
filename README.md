# Test sources for [gn-build](https://github.com/dyu/gn-build) originally based from timniederhausen's [testsrc](https://github.com/timniederhausen/gn-build/tree/testsrc)

1. `git clone --depth 1 --single-branch -b ns https://github.com/dyu/gn-build`

2. On linux:
   ```sh
   gn gen gn-out --args='gcc_cc="gcc" gcc_cxx="g++" symbol_level=0 is_debug=false is_clang=false is_official_build=true'
   ```
   On windows:
   ```sh
   gn gen gn-out --args="visual_studio_path=\"C:\\Program Files (x86)\\Microsoft Visual Studio 14.0\" visual_studio_version=\"2015\" symbol_level=0 is_debug=false is_clang=false is_official_build=true"
   ```

3. `ninja -C gn-out`
