#Add Subdirectories
add_subdirectory(HazeDumper)
add_subdirectory(MemManager)
add_subdirectory(Cheats)

#Link MemMan to Cheats
target_link_libraries(Cheats MemMan)
target_link_libraries(Cheats HazeImporter)

#Create exe
add_executable(Anti-VAC main.cpp)

target_link_libraries(Anti-VAC Cheats)

