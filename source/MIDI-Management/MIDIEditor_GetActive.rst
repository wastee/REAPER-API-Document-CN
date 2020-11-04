MIDIEditor_GetActive
=============================================
.. raw:: html

    <span>
        提交者: 当归蛋&nbsp;&nbsp;&nbsp;&nbsp;提交日期: 2020-10-23
    </span>
    <p></p>
    
``MIDIEditor_GetActive``\()
   获取当前激活的MIDI编辑器窗口。

      :参数:
            无

      :返回:
            HWND

   .. note::
         在MIDI编辑器中运行脚本，最开始应该运行这个API来定位到当前激活的MIDI编辑器，通常MIDIEditor_GetTake运行在后。


         
   .. rubric:: 范例
   .. code-block:: lua
      :caption: Lua:

         editor = reaper.MIDIEditor_GetActive()

   .. code-block:: python
      :caption: Python:

         MediaItem_Take





