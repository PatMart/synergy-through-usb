# synergy -- mouse and keyboard sharing utility
# Copyright (C) 2012 Bolton Software Ltd.
# Copyright (C) 2011 Nick Bolton
# 
# This package is free software; you can redistribute it and/or
# modify it under the terms of the GNU General Public License
# found in the file COPYING that should have accompanied this file.
# 
# This package is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.

include_directories(
	../../tools/gtest-1.6.0
	../../tools/gtest-1.6.0/include
	../../tools/gmock-1.6.0
	../../tools/gmock-1.6.0/include)
	
add_library(gtest STATIC ../../tools/gtest-1.6.0/src/gtest-all.cc)
add_library(gmock STATIC ../../tools/gmock-1.6.0/src/gmock-all.cc)

add_subdirectory(integtests)
add_subdirectory(unittests)
