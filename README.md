# Assets

Public asset host for project pages.

## Layout

```
<project>/<kind>/<files>
```

## invaria

Colored `.ply` point clouds for the Invaria project page. Per scene:

- `gt.ply` — ground-truth segmentation
- `<model>_<res>.ply` — predictions; `<model>` ∈ {spunet, ptv3, sonata, utonia, ours}, `<res>` ∈ {2cm, 6cm}

Both 2cm and 6cm predictions are projected back to the original point cloud, so the two halves of each split viewer share geometry and differ only in per-point labels.
