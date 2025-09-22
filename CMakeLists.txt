cmake_minimum_required(VERSION 3.5)

project(VendingMachine LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(VendingMachine main.cpp soda.cpp vendingmachine.cpp soda.h vendingmachine.h)

include(GNUInstallDirs)
install(TARGETS VendingMachine
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
