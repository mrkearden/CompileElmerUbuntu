# CompileElmerUbuntu

mkdir elmer  
cd elmer  
git clone https://github.com/ElmerCSC/elmerfem.git  
sudo apt install git cmake build-essential gfortran libopenmpi-dev libblas-dev liblapack-dev  
sudo apt install libqt4-dev libqwt-dev  
sudo apt install libqt5opengl5-dev  
sudo apt install qtscript5-dev  
sudo apt install libqt5svg5-dev  
mkdir build  
cd build  
cmake -DWITH_ELMERGUI:BOOL=TRUE -DWITH_MPI:BOOL=FALSE -DCMAKE_INSTALL_PREFIX=../install ../elmerfem  
make install  
