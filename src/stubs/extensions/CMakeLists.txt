#=============================================================================
#  MuseScore
#  Music Composition & Notation
#
#  Copyright (C) 2020 MuseScore BVBA and others
#
#  This program is free software; you can redistribute it and/or modify
#  it under the terms of the GNU General Public License version 2.
#
#  This program is distributed in the hope that it will be useful,
#  but WITHOUT ANY WARRANTY; without even the implied warranty of
#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
#  GNU General Public License for more details.
#
#  You should have received a copy of the GNU General Public License
#  along with this program; if not, write to the Free Software
#  Foundation, Inc., 675 Mass Ave, Cambridge, MA 02139, USA.
#=============================================================================

set(MODULE extensions)

set(MODULE_QRC extensions.qrc)

set(MODULE_QML_IMPORT ${CMAKE_CURRENT_LIST_DIR}/qml )

set(MODULE_SRC
    ${CMAKE_CURRENT_LIST_DIR}/extensionsstubmodule.cpp
    ${CMAKE_CURRENT_LIST_DIR}/extensionsstubmodule.h
    ${CMAKE_CURRENT_LIST_DIR}/extensionsservicestub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/extensionsservicestub.h
    ${CMAKE_CURRENT_LIST_DIR}/extensionsconfigurationstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/extensionsconfigurationstub.h
    ${CMAKE_CURRENT_LIST_DIR}/extensionunpackerstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/extensionunpackerstub.h
    )

include(${PROJECT_SOURCE_DIR}/build/module.cmake)

