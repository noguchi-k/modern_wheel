#
# Modern Wheel : all the things that shouldn't be reinvented from one project to the other
#
# The MIT License (MIT)
# 
# Copyright (C) 2015  Massimiliano Culpo
# 
# Permission is hereby granted, free of charge, to any person obtaining a copy
# of this software and associated documentation files (the "Software"), to deal
# in the Software without restriction, including without limitation the rights
# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
# copies of the Software, and to permit persons to whom the Software is
# furnished to do so, subject to the following conditions:
# 
# The above copyright notice and this permission notice shall be included in all
# copies or substantial portions of the Software.
# 
# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
# SOFTWARE.
# 

SET( 
  MWHEEL_HEADERS_LOCAL
  ${CMAKE_CURRENT_SOURCE_DIR}/mwheel/utility.h
  ${CMAKE_CURRENT_SOURCE_DIR}/mwheel/expected.h
  ${CMAKE_CURRENT_SOURCE_DIR}/mwheel/plugin.h
  ${CMAKE_CURRENT_SOURCE_DIR}/mwheel/serializable_object.h
  ${CMAKE_CURRENT_SOURCE_DIR}/mwheel/memento_originator.h
  ${CMAKE_CURRENT_SOURCE_DIR}/mwheel/composite_base.h
  ${CMAKE_CURRENT_SOURCE_DIR}/mwheel/singleton.h
  ${CMAKE_CURRENT_SOURCE_DIR}/mwheel/prototype_factory.h
  ${CMAKE_CURRENT_SOURCE_DIR}/mwheel/dlmanager.h  
)

SET( 
  MWHEEL_HEADERS
  ${MWHEEL_HEADERS_LOCAL}
  PARENT_SCOPE
)
  
INSTALL( 
  FILES ${MWHEEL_HEADERS_LOCAL}
  DESTINATION "include/mwheel"
)