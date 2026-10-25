android_etc/v1_6  —  NOT “version 6 only”
=====================================

  v1_6  = client branch name (fixed in the URL path)
  1, 2, 3 … 14  = bundle VERSION folders inside this directory

The game loads portraits/thumbs from:
  .../android_etc/v1_6/{version}/{name}.assetBundle

Folders 7–14 may have been GAP-FILLED (copies of v6) by fill_android_etc_version_gaps.py.
That is NOT the same as real newer CDN builds.

To fetch real newest files from CDN:
  cd "..\..\..\..\..\..\.."
  python fetch_real_newest_bundles.py --path android_etc --v-max 20 --yes

World/dragon 3D bundles use Android/{version}/ (separate folder), not this tree.
