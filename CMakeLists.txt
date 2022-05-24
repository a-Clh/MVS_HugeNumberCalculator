cmake_minimum_required(VERSION 3.21)
project(MVS_HugeNumberCalculator)

set(CMAKE_C_STANDARD 11)

include_directories(DataTypes)
include_directories(IHMHugeNumber)
include_directories(UseHugeNumber/Operator)
include_directories(UseHugeNumber/Type)

add_executable(MVS_HugeNumberCalculator
        DataTypes/DoublyLinkedList.c
        DataTypes/DoublyLinkedList.h
        IHMHugeNumber/ScanHugeNumber.c
        IHMHugeNumber/ScanHugeNumber.h
        IHMHugeNumber/ShowHugeNumber.c
        IHMHugeNumber/ShowHugeNumber.h
        UseHugeNumber/Operator/HugeFloatOperator.c
        UseHugeNumber/Operator/HugeFloatOperator.h
        UseHugeNumber/Operator/HugeIntOperator.c
        UseHugeNumber/Operator/HugeIntOperator.h
        UseHugeNumber/Operator/HugeUnsignedIntOperator.c
        UseHugeNumber/Operator/HugeUnsignedIntOperator.h
        UseHugeNumber/Type/HugeFloat.c
        UseHugeNumber/Type/HugeFloat.h
        UseHugeNumber/Type/HugeInt.c
        UseHugeNumber/Type/HugeInt.h
        UseHugeNumber/Type/HugeUnsignedInt.c
        UseHugeNumber/Type/HugeUnsignedInt.h
        main.c)
