fips_begin_lib(glyphy)
    add_definitions(-DPKGDATADIR=".")
    include_directories(glyphy/src)
    include_directories(shaders)
    fips_files(
        glyphy/src/glyphy-arc-bezier.hh
        glyphy/src/glyphy-arc.cc
        glyphy/src/glyphy-arcs-bezier.hh
        glyphy/src/glyphy-arcs.cc
        glyphy/src/glyphy-blob.cc
        # glyphy/src/glyphy-common-glsl.h
        shaders/glyphy-sdf-glsl.h
        glyphy/src/glyphy-common.hh
        glyphy/src/glyphy-extents.cc
        glyphy/src/glyphy-freetype.h
        glyphy/src/glyphy-geometry.hh
        glyphy/src/glyphy-outline.cc
        # glyphy/src/glyphy-sdf-glsl.h
        shaders/glyphy-common-glsl.h
        glyphy/src/glyphy-sdf.cc
        glyphy/src/glyphy-shaders.cc
        glyphy/src/glyphy.h

        # shaders/demo-atlas-glsl.h
        # shaders/demo-fshader-glsl.h
        # shaders/demo-vshader-glsl.h

    )
fips_end_lib()
