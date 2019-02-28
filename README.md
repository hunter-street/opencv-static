~/mixo_devtools/cmake-3.14.0-rc2-Linux-x86_64/bin/cmake \
    -D BUILD_DOCS=OFF \
    -D BUILD_EXAMPLES=OFF \
    -D BUILD_opencv_apps=OFF \
    -D BUILD_opencv_python2=OFF \
    -D BUILD_opencv_python3=OFF \
    -D BUILD_PERF_TESTS=OFF \
    -D BUILD_SHARED_LIBS=OFF \
    -D BUILD_TESTS=OFF \
    -D CMAKE_BUILD_TYPE=RELEASE \
    -D ENABLE_PRECOMPILED_HEADERS=OFF \
    -D FORCE_VTK=OFF \
    -D WITH_FFMPEG=OFF \
    -D WITH_GDAL=OFF \
    -D WITH_IPP=OFF \
    -D WITH_OPENEXR=OFF \
    -D WITH_OPENGL=OFF \
    -D WITH_QT=OFF \
    -D WITH_TBB=OFF \
    -D WITH_XINE=OFF \
    -D BUILD_JPEG=ON  \
    -D BUILD_TIFF=ON \
    -D BUILD_PNG=ON \
    -D CMAKE_CXX_FLAGS="-std=c++11" \
    -D ENABLE_CXX11=ON \
    -D WITH_GTK=ON \
    -D CMAKE_INSTALL_PREFIX=/media/dalong/F2AA43F8AA43B7BD/Users/dalon/Projects/study/opencv/build_in_linux/opencv_install \
  .. \

make -j4
make install

cd <DisplayImageProjRoot>
mkdir build && cd build
~/mixo_devtools/cmake-3.14.0-rc2-Linux-x86_64/bin/cmake ..
make


WITH_GTK=ON otherwise error when run ./DisplayImage
If you are on Ubuntu or Debian, install libgtk2.0-dev and pkg-config, then re-run cmake or configure script in function 'cvNamedWindow'

Some similars:
-D WITH_QT=ON -D WITH_OPENGL=ON 
