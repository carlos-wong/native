set(SRCS
  bits/bits.cpp
  bits/varint.cpp
  random/perlin.cpp
  hash/hash.cpp
)

set(SRCS ${SRCS})

add_library(util STATIC ${SRCS})

if(UNIX)
  add_definitions(-fPIC)
endif(UNIX)

