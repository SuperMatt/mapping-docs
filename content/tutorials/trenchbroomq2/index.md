+++
title = 'Configure TrenchBroom for Quake 2 Mapping'
date = 2024-08-15T11:20:29+01:00
draft = false
+++


# Compiling

## Tools

### Details

Name: Quake 2 RE (fast)

Working Directory: `${GAME_DIR_PATH}\baseq2\maps`

### Run Tool

Tool Path: `E:/Matthew/Quake 2 Maps/ericw-tools/bin/qbsp.exe`

Parameters: `-nostat -nopercent -q2bsp -gamedir "${GAME_DIR_PATH}" -basedir "${GAME_DIR_PATH}\baseq2" "${MAP_DIR_PATH}\${MAP_FULL_NAME}" "${GAME_DIR_PATH}\baseq2\maps\${MAP_BASE_NAME}.bsp"`

### Run Tool

Tool Path: `E:/Matthew/Quake 2 Maps/ericw-tools/bin/vis.exe`

Parameters: `-gamedir "${GAME_DIR_PATH}" -basedir "${GAME_DIR_PATH}\baseq2" "${GAME_DIR_PATH}\baseq2\maps\${MAP_BASE_NAME}.bsp"`

### Run Tool

Tool Path: `E:/Matthew/Quake 2 Maps/ericw-tools/bin/light.exe`

Parameters: `-nostat -dirt -world_units_per_luxel 24 -wrnormals -novanilla -lightgrid -lightgrid_dist 64 64 64 -gamedir "${GAME_DIR_PATH}" -basedir "${GAME_DIR_PATH}\baseq2" "${GAME_DIR_PATH}\baseq2\maps\${MAP_BASE_NAME}.bsp"`


# Launch Parameters

## Parameters

Deathmatch: `-applaunch 2320 -skipmovies +set flushmap 1 +map ${MAP_BASE_NAME} +set deathmatch 1 +set g_dm_no_fall_damage 1 +set cheats 1 +set g_weapon_respawn_time 1 +set fraglimit 20`

Singleplayer: `-applaunch 2320 -skipmovies +set flushmap 1 +map ${MAP_BASE_NAME}`
