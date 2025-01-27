:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/AudioStreamPlaybackPolyphonic.xml.

.. _class_AudioStreamPlaybackPolyphonic:

AudioStreamPlaybackPolyphonic
=============================

**继承：** :ref:`AudioStreamPlayback<class_AudioStreamPlayback>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

:ref:`AudioStreamPolyphonic<class_AudioStreamPolyphonic>` 的播放实例。

.. rst-class:: classref-introduction-group

描述
----

:ref:`AudioStreamPolyphonic<class_AudioStreamPolyphonic>` 的播放实例。设置 :ref:`AudioStreamPlayer<class_AudioStreamPlayer>`\ 、\ :ref:`AudioStreamPlayer2D<class_AudioStreamPlayer2D>` 或 :ref:`AudioStreamPlayer3D<class_AudioStreamPlayer3D>` 的 ``stream`` 属性后，可以通过调用 :ref:`AudioStreamPlayer.get_stream_playback<class_AudioStreamPlayer_method_get_stream_playback>`\ 、\ :ref:`AudioStreamPlayer2D.get_stream_playback<class_AudioStreamPlayer2D_method_get_stream_playback>` 或 :ref:`AudioStreamPlayer3D.get_stream_playback<class_AudioStreamPlayer3D_method_get_stream_playback>` 方法获取播放实例。

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>` | :ref:`is_stream_playing<class_AudioStreamPlaybackPolyphonic_method_is_stream_playing>` **(** :ref:`int<class_int>` stream **)** |const|                                                                                                                        |
   +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`   | :ref:`play_stream<class_AudioStreamPlaybackPolyphonic_method_play_stream>` **(** :ref:`AudioStream<class_AudioStream>` stream, :ref:`float<class_float>` from_offset=0, :ref:`float<class_float>` volume_db=0, :ref:`float<class_float>` pitch_scale=1.0 **)** |
   +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                    | :ref:`set_stream_pitch_scale<class_AudioStreamPlaybackPolyphonic_method_set_stream_pitch_scale>` **(** :ref:`int<class_int>` stream, :ref:`float<class_float>` pitch_scale **)**                                                                               |
   +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                    | :ref:`set_stream_volume<class_AudioStreamPlaybackPolyphonic_method_set_stream_volume>` **(** :ref:`int<class_int>` stream, :ref:`float<class_float>` volume_db **)**                                                                                           |
   +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                    | :ref:`stop_stream<class_AudioStreamPlaybackPolyphonic_method_stop_stream>` **(** :ref:`int<class_int>` stream **)**                                                                                                                                            |
   +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

常量
----

.. _class_AudioStreamPlaybackPolyphonic_constant_INVALID_ID:

.. rst-class:: classref-constant

**INVALID_ID** = ``-1``

无法为播放分配一个流时由 :ref:`play_stream<class_AudioStreamPlaybackPolyphonic_method_play_stream>` 返回。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_AudioStreamPlaybackPolyphonic_method_is_stream_playing:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **is_stream_playing** **(** :ref:`int<class_int>` stream **)** |const|

与整数 ID 关联的流仍在播放时返回 true。请检查 :ref:`play_stream<class_AudioStreamPlaybackPolyphonic_method_play_stream>` 以获取有关此 ID 何时失效的信息。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlaybackPolyphonic_method_play_stream:

.. rst-class:: classref-method

:ref:`int<class_int>` **play_stream** **(** :ref:`AudioStream<class_AudioStream>` stream, :ref:`float<class_float>` from_offset=0, :ref:`float<class_float>` volume_db=0, :ref:`float<class_float>` pitch_scale=1.0 **)**

以给定的偏移量、音量和音高播放 :ref:`AudioStream<class_AudioStream>`\ 。播放立即开始。

返回值是与该播放流关联的唯一整数 ID，可用于控制该播放流。

当流结束（不循环）、\ **AudioStreamPlaybackPolyphonic** 停止或 :ref:`stop_stream<class_AudioStreamPlaybackPolyphonic_method_stop_stream>` 被调用时，该 ID 将失效。

如果当前播放的流的数量等于 :ref:`AudioStreamPolyphonic.polyphony<class_AudioStreamPolyphonic_property_polyphony>`\ ，则该函数将返回 :ref:`INVALID_ID<class_AudioStreamPlaybackPolyphonic_constant_INVALID_ID>`\ 。如果需要更大的最大复音数，请提高该值。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlaybackPolyphonic_method_set_stream_pitch_scale:

.. rst-class:: classref-method

void **set_stream_pitch_scale** **(** :ref:`int<class_int>` stream, :ref:`float<class_float>` pitch_scale **)**

改变流的音阶。\ ``stream`` 参数是一个由 :ref:`play_stream<class_AudioStreamPlaybackPolyphonic_method_play_stream>` 返回的整数 ID。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlaybackPolyphonic_method_set_stream_volume:

.. rst-class:: classref-method

void **set_stream_volume** **(** :ref:`int<class_int>` stream, :ref:`float<class_float>` volume_db **)**

改变流的音量（单位：db）。\ ``stream`` 参数是一个由 :ref:`play_stream<class_AudioStreamPlaybackPolyphonic_method_play_stream>` 返回的整数 ID。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlaybackPolyphonic_method_stop_stream:

.. rst-class:: classref-method

void **stop_stream** **(** :ref:`int<class_int>` stream **)**

停止某个流。\ ``stream`` 参数是由 :ref:`play_stream<class_AudioStreamPlaybackPolyphonic_method_play_stream>` 返回的整数 ID，在调用这个函数后失效。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
