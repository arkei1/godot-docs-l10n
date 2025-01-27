:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/AudioEffectPanner.xml.

.. _class_AudioEffectPanner:

AudioEffectPanner
=================

**继承：** :ref:`AudioEffect<class_AudioEffect>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

向音频总线添加一个声像器音频效果。向左或向右声像移动声音。

.. rst-class:: classref-introduction-group

描述
----

决定向左右总线发送的音频信号量。

.. rst-class:: classref-introduction-group

教程
----

- :doc:`音频总线 <../tutorials/audio/audio_buses>`

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +---------------------------+--------------------------------------------------+---------+
   | :ref:`float<class_float>` | :ref:`pan<class_AudioEffectPanner_property_pan>` | ``0.0`` |
   +---------------------------+--------------------------------------------------+---------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_AudioEffectPanner_property_pan:

.. rst-class:: classref-property

:ref:`float<class_float>` **pan** = ``0.0``

.. rst-class:: classref-property-setget

- void **set_pan** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_pan** **(** **)**

声像位置。值的范围可以从 -1（完全左）到1（完全右）。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
