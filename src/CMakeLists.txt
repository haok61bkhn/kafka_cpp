find_package(CppKafka REQUIRED)
# target_link_libraries(kafka CppKafka::cppkafka)
set(PROGS consumer
          producer
          
)

foreach(item ${PROGS})
    add_executable(${item} "${item}.cpp")
    target_link_libraries(${item} CppKafka::cppkafka)    
endforeach(item)