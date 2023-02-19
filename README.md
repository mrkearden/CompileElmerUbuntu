# CompileElmerUbuntu

mkdir elmer  
cd elmer  
git clone https://github.com/ElmerCSC/elmerfem.git  
sudo apt install git cmake build-essential gfortran libopenmpi-dev libblas-dev liblapack-dev  
sudo apt install libqt4-dev libqwt-dev  
sudo apt install libqt5opengl5-dev  
sudo apt install qtscript5-dev  
sudo apt install libqt5svg5-dev  
sudo apt install qt5-default qtscript5-dev libqwt-qt5-dev  
sudo apt install cmake cmake-qt5 gcc g++ gfortran qt5-default qtscript5-dev libqwt-qt5-dev libmpich-dev libblas-dev liblapack-dev libqt5svg5-dev   libnetcdff-dev libmetis-dev libparmetis-dev libmumps-dev netcdf-bin  
sudo apt install lua5.3  
sudo apt-get install libmumps-dev  
sudo apt-get install libparmetis-dev  
mkdir build  
cd build  
cmake -DWITH_QT5=TRUE -DWITH_ELMERGUI:BOOL=TRUE -DWITH_MPI:BOOL=TRUE -DWITH_Mumps:BOOL=TRUE -DWITH_LUA:BOOL=TRUE -DCMAKE_INSTALL_PREFIX=../install ../elmerfem  
make install  
