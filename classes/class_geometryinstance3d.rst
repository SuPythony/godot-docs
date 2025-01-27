:github_url: hide

.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the GeometryInstance3D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_GeometryInstance3D:

GeometryInstance3D
==================

**Inherits:** :ref:`VisualInstance3D<class_VisualInstance3D>` **<** :ref:`Node3D<class_Node3D>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`CPUParticles3D<class_CPUParticles3D>`, :ref:`CSGShape3D<class_CSGShape3D>`, :ref:`GPUParticles3D<class_GPUParticles3D>`, :ref:`MeshInstance3D<class_MeshInstance3D>`, :ref:`MultiMeshInstance3D<class_MultiMeshInstance3D>`, :ref:`SpriteBase3D<class_SpriteBase3D>`

Base node for geometry-based visual instances.

Description
-----------

Base node for geometry-based visual instances. Shares some common functionality like visibility and custom materials.

Properties
----------

+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+
| :ref:`ShadowCastingSetting<enum_GeometryInstance3D_ShadowCastingSetting>` | :ref:`cast_shadow<class_GeometryInstance3D_property_cast_shadow>`                                     | ``1``     |
+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>`                                                 | :ref:`extra_cull_margin<class_GeometryInstance3D_property_extra_cull_margin>`                         | ``0.0``   |
+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+
| :ref:`LightmapScale<enum_GeometryInstance3D_LightmapScale>`               | :ref:`gi_lightmap_scale<class_GeometryInstance3D_property_gi_lightmap_scale>`                         | ``0``     |
+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+
| :ref:`GIMode<enum_GeometryInstance3D_GIMode>`                             | :ref:`gi_mode<class_GeometryInstance3D_property_gi_mode>`                                             | ``0``     |
+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`                                                   | :ref:`ignore_occlusion_culling<class_GeometryInstance3D_property_ignore_occlusion_culling>`           | ``false`` |
+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>`                                                 | :ref:`lod_bias<class_GeometryInstance3D_property_lod_bias>`                                           | ``1.0``   |
+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+
| :ref:`Material<class_Material>`                                           | :ref:`material_override<class_GeometryInstance3D_property_material_override>`                         |           |
+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>`                                                 | :ref:`visibility_range_begin<class_GeometryInstance3D_property_visibility_range_begin>`               | ``0.0``   |
+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>`                                                 | :ref:`visibility_range_begin_margin<class_GeometryInstance3D_property_visibility_range_begin_margin>` | ``0.0``   |
+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>`                                                 | :ref:`visibility_range_end<class_GeometryInstance3D_property_visibility_range_end>`                   | ``0.0``   |
+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>`                                                 | :ref:`visibility_range_end_margin<class_GeometryInstance3D_property_visibility_range_end_margin>`     | ``0.0``   |
+---------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-----------+

Methods
-------

+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Variant<class_Variant>` | :ref:`get_shader_instance_uniform<class_GeometryInstance3D_method_get_shader_instance_uniform>` **(** :ref:`StringName<class_StringName>` uniform **)** |const|                              |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`set_custom_aabb<class_GeometryInstance3D_method_set_custom_aabb>` **(** :ref:`AABB<class_AABB>` aabb **)**                                                                             |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`set_shader_instance_uniform<class_GeometryInstance3D_method_set_shader_instance_uniform>` **(** :ref:`StringName<class_StringName>` uniform, :ref:`Variant<class_Variant>` value **)** |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Enumerations
------------

.. _enum_GeometryInstance3D_ShadowCastingSetting:

.. _class_GeometryInstance3D_constant_SHADOW_CASTING_SETTING_OFF:

.. _class_GeometryInstance3D_constant_SHADOW_CASTING_SETTING_ON:

.. _class_GeometryInstance3D_constant_SHADOW_CASTING_SETTING_DOUBLE_SIDED:

.. _class_GeometryInstance3D_constant_SHADOW_CASTING_SETTING_SHADOWS_ONLY:

enum **ShadowCastingSetting**:

- **SHADOW_CASTING_SETTING_OFF** = **0** --- Will not cast any shadows.

- **SHADOW_CASTING_SETTING_ON** = **1** --- Will cast shadows from all visible faces in the GeometryInstance3D.

Will take culling into account, so faces not being rendered will not be taken into account when shadow casting.

- **SHADOW_CASTING_SETTING_DOUBLE_SIDED** = **2** --- Will cast shadows from all visible faces in the GeometryInstance3D.

Will not take culling into account, so all faces will be taken into account when shadow casting.

- **SHADOW_CASTING_SETTING_SHADOWS_ONLY** = **3** --- Will only show the shadows casted from this object.

In other words, the actual mesh will not be visible, only the shadows casted from the mesh will be.

----

.. _enum_GeometryInstance3D_GIMode:

.. _class_GeometryInstance3D_constant_GI_MODE_DISABLED:

.. _class_GeometryInstance3D_constant_GI_MODE_BAKED:

.. _class_GeometryInstance3D_constant_GI_MODE_DYNAMIC:

enum **GIMode**:

- **GI_MODE_DISABLED** = **0**

- **GI_MODE_BAKED** = **1**

- **GI_MODE_DYNAMIC** = **2**

----

.. _enum_GeometryInstance3D_LightmapScale:

.. _class_GeometryInstance3D_constant_LIGHTMAP_SCALE_1X:

.. _class_GeometryInstance3D_constant_LIGHTMAP_SCALE_2X:

.. _class_GeometryInstance3D_constant_LIGHTMAP_SCALE_4X:

.. _class_GeometryInstance3D_constant_LIGHTMAP_SCALE_8X:

.. _class_GeometryInstance3D_constant_LIGHTMAP_SCALE_MAX:

enum **LightmapScale**:

- **LIGHTMAP_SCALE_1X** = **0**

- **LIGHTMAP_SCALE_2X** = **1**

- **LIGHTMAP_SCALE_4X** = **2**

- **LIGHTMAP_SCALE_8X** = **3**

- **LIGHTMAP_SCALE_MAX** = **4**

Property Descriptions
---------------------

.. _class_GeometryInstance3D_property_cast_shadow:

- :ref:`ShadowCastingSetting<enum_GeometryInstance3D_ShadowCastingSetting>` **cast_shadow**

+-----------+---------------------------------+
| *Default* | ``1``                           |
+-----------+---------------------------------+
| *Setter*  | set_cast_shadows_setting(value) |
+-----------+---------------------------------+
| *Getter*  | get_cast_shadows_setting()      |
+-----------+---------------------------------+

The selected shadow casting flag. See :ref:`ShadowCastingSetting<enum_GeometryInstance3D_ShadowCastingSetting>` for possible values.

----

.. _class_GeometryInstance3D_property_extra_cull_margin:

- :ref:`float<class_float>` **extra_cull_margin**

+-----------+------------------------------+
| *Default* | ``0.0``                      |
+-----------+------------------------------+
| *Setter*  | set_extra_cull_margin(value) |
+-----------+------------------------------+
| *Getter*  | get_extra_cull_margin()      |
+-----------+------------------------------+

The extra distance added to the GeometryInstance3D's bounding box (:ref:`AABB<class_AABB>`) to increase its cull box.

----

.. _class_GeometryInstance3D_property_gi_lightmap_scale:

- :ref:`LightmapScale<enum_GeometryInstance3D_LightmapScale>` **gi_lightmap_scale**

+-----------+---------------------------+
| *Default* | ``0``                     |
+-----------+---------------------------+
| *Setter*  | set_lightmap_scale(value) |
+-----------+---------------------------+
| *Getter*  | get_lightmap_scale()      |
+-----------+---------------------------+

----

.. _class_GeometryInstance3D_property_gi_mode:

- :ref:`GIMode<enum_GeometryInstance3D_GIMode>` **gi_mode**

+-----------+--------------------+
| *Default* | ``0``              |
+-----------+--------------------+
| *Setter*  | set_gi_mode(value) |
+-----------+--------------------+
| *Getter*  | get_gi_mode()      |
+-----------+--------------------+

----

.. _class_GeometryInstance3D_property_ignore_occlusion_culling:

- :ref:`bool<class_bool>` **ignore_occlusion_culling**

+-----------+-------------------------------------+
| *Default* | ``false``                           |
+-----------+-------------------------------------+
| *Setter*  | set_ignore_occlusion_culling(value) |
+-----------+-------------------------------------+
| *Getter*  | is_ignoring_occlusion_culling()     |
+-----------+-------------------------------------+

----

.. _class_GeometryInstance3D_property_lod_bias:

- :ref:`float<class_float>` **lod_bias**

+-----------+---------------------+
| *Default* | ``1.0``             |
+-----------+---------------------+
| *Setter*  | set_lod_bias(value) |
+-----------+---------------------+
| *Getter*  | get_lod_bias()      |
+-----------+---------------------+

----

.. _class_GeometryInstance3D_property_material_override:

- :ref:`Material<class_Material>` **material_override**

+----------+------------------------------+
| *Setter* | set_material_override(value) |
+----------+------------------------------+
| *Getter* | get_material_override()      |
+----------+------------------------------+

The material override for the whole geometry.

If a material is assigned to this property, it will be used instead of any material set in any material slot of the mesh.

----

.. _class_GeometryInstance3D_property_visibility_range_begin:

- :ref:`float<class_float>` **visibility_range_begin**

+-----------+-----------------------------------+
| *Default* | ``0.0``                           |
+-----------+-----------------------------------+
| *Setter*  | set_visibility_range_begin(value) |
+-----------+-----------------------------------+
| *Getter*  | get_visibility_range_begin()      |
+-----------+-----------------------------------+

Starting distance from which the GeometryInstance3D will be visible, taking :ref:`visibility_range_begin_margin<class_GeometryInstance3D_property_visibility_range_begin_margin>` into account as well. The default value of 0 is used to disable the range check.

----

.. _class_GeometryInstance3D_property_visibility_range_begin_margin:

- :ref:`float<class_float>` **visibility_range_begin_margin**

+-----------+------------------------------------------+
| *Default* | ``0.0``                                  |
+-----------+------------------------------------------+
| *Setter*  | set_visibility_range_begin_margin(value) |
+-----------+------------------------------------------+
| *Getter*  | get_visibility_range_begin_margin()      |
+-----------+------------------------------------------+

Margin for the :ref:`visibility_range_begin<class_GeometryInstance3D_property_visibility_range_begin>` threshold. The GeometryInstance3D will only change its visibility state when it goes over or under the :ref:`visibility_range_begin<class_GeometryInstance3D_property_visibility_range_begin>` threshold by this amount.

----

.. _class_GeometryInstance3D_property_visibility_range_end:

- :ref:`float<class_float>` **visibility_range_end**

+-----------+---------------------------------+
| *Default* | ``0.0``                         |
+-----------+---------------------------------+
| *Setter*  | set_visibility_range_end(value) |
+-----------+---------------------------------+
| *Getter*  | get_visibility_range_end()      |
+-----------+---------------------------------+

Distance from which the GeometryInstance3D will be hidden, taking :ref:`visibility_range_end_margin<class_GeometryInstance3D_property_visibility_range_end_margin>` into account as well. The default value of 0 is used to disable the range check..

----

.. _class_GeometryInstance3D_property_visibility_range_end_margin:

- :ref:`float<class_float>` **visibility_range_end_margin**

+-----------+----------------------------------------+
| *Default* | ``0.0``                                |
+-----------+----------------------------------------+
| *Setter*  | set_visibility_range_end_margin(value) |
+-----------+----------------------------------------+
| *Getter*  | get_visibility_range_end_margin()      |
+-----------+----------------------------------------+

Margin for the :ref:`visibility_range_end<class_GeometryInstance3D_property_visibility_range_end>` threshold. The GeometryInstance3D will only change its visibility state when it goes over or under the :ref:`visibility_range_end<class_GeometryInstance3D_property_visibility_range_end>` threshold by this amount.

Method Descriptions
-------------------

.. _class_GeometryInstance3D_method_get_shader_instance_uniform:

- :ref:`Variant<class_Variant>` **get_shader_instance_uniform** **(** :ref:`StringName<class_StringName>` uniform **)** |const|

----

.. _class_GeometryInstance3D_method_set_custom_aabb:

- void **set_custom_aabb** **(** :ref:`AABB<class_AABB>` aabb **)**

Overrides the bounding box of this node with a custom one. To remove it, set an :ref:`AABB<class_AABB>` with all fields set to zero.

----

.. _class_GeometryInstance3D_method_set_shader_instance_uniform:

- void **set_shader_instance_uniform** **(** :ref:`StringName<class_StringName>` uniform, :ref:`Variant<class_Variant>` value **)**

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
