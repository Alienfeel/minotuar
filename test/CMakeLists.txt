
include_directories(
  ../source
  ${Boost_INCLUDE_DIRS}
  ${ALLSPARK_INCLUDE_DIRS}
)

link_libraries(
  ${Boost_LIBRARIES}
  ${MINOTAUR_LIBRARIES}
  pthread
  rt
)

add_executable(t_local
  t_local.cpp)

#add_executable(t_lock_free_ring
#  t_lock_free_ring.cpp)

add_executable(t_event_loop
  t_event_loop.cpp)

add_executable(t_static_list_pool
  t_static_list_pool.cpp)