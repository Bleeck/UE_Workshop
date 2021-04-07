# Session 3
[Back to workshop](https://github.com/Bleeck/UE_Workshop)

---

* [Vector Math Helper](https://github.com/Bleeck/UE_Workshop/blob/master/Session_3.md#vector_math_helper)
* [Spline Component](https://github.com/Bleeck/UE_Workshop/blob/master/Session_3.md#spline_component)
---

### [Vector Math Helper](https://github.com/Bleeck/UE_Workshop/blob/main/Session_3.md)
    In the project you can find the Vector Math Helper (Content/VectorMathHelper/
      VectorMathHelper).
    It is a helper object designed to give an interactive example for the most
    common vector math operations.
    You can tweak the parameters in the "Default" section:
      - Operation - allows you to select the current operation (add/multiply/dot/cross)
      - Normalize A/B/Result - Normalizes the vectors (ie: it makes the vector have length 1)
      - Scalar - the value of the number by which vector A is multiplied when doing
      the multiplication Operation
      - Print Acos - during the Dot operation the helper prints the result. This
      will make the tool apply an ArcCosinus on that value. The resulting number
      is the value of the angle (in degrees) between the 2 vectors.

---
###[Spline Component](https://github.com/Bleeck/UE_Workshop/blob/main/Session_3.md)    
    Unreal splines work by interpolating positions between consecutive points.
    Splines are ordered. They have a beginning and an end. The spline also contains
    a set of points that define it's shape.
    Each point contains the transform of the specified point, and also the tangents
    of the spline at that point.
    The "In Tangent" controls the entry direction of the spline into that point and
    the "Out Tangent" controls the exit direction of the spline.

    Useful functions:
      - Get Spline Length : get the length of the spline
      - Get Location At Distance Along Spline: get the location by passing in
      the distance along the spline at which you want to sample the location
      - Set Location at Spline Point : set the location of an already added spline point
      - Get Number of Spline Points

[Splines Documentation](https://docs.unrealengine.com/en-US/BuildingWorlds/BlueprintSplines/index.html)

---




---
[Back to workshop](https://github.com/Bleeck/UE_Workshop)
