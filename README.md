Quakespasm-for-GL4ES
=====================

A port of Quakespasm that supports the use of GL4ES for OpenGL ES systems originally modified by jfgomez21.

### This modified version adds support for use with GL4ES by ptitseb which can be found at:

[https://github.com/ptitSeb/gl4es](https://github.com/ptitSeb/gl4es)

### To compile for Linux Ubuntu/Debian derivitives make sure you have the necessary dependencies installed:

```bash
sudo apt install libmikmod-dev flac libsdl2-dev libvorbis-dev libogg-dev
```

### Then build with:

```bash
cd Quake
make -j#  (replace # with the number of CPU cores/threads in your system for faster compiling!)
```

Be sure to copy both 'quakespasm' and 'quakespasm.pak' to your Quake folder.
Follow the usual regimen for populating id1, hipnotic, dopa, and rogue directories with pak files and music files.

### To run on Anbernic devices after building both quakespasm and gl4es:
```bash
LD_LIBRARY_PATH=/path/to/gl4es LIBGL_GL=15 LIBGL_NOTEST=1 LIBGL_GAMMA=1.0 ./quakespasm
```
