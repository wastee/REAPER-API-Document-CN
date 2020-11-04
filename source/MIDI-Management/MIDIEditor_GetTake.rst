MIDIEditor_GetTake
=============================================
.. raw:: html

    <span>
        提交者: 当归蛋&nbsp;&nbsp;&nbsp;&nbsp;提交日期: 2020-10-23
    </span>
    <p></p>
    
``MIDIEditor_GetTake``\(*HWND*)
   获取当前MIDI编辑器中当前正在编辑的take（片段）。

      :参数:
         **HWND**
            先用 MIDIEditor_GetActive 获取当前MIDI编辑器。

      :返回:
            HWND

   .. note::
         通常运行在 	MIDIEditor_GetActive 之后


         
   .. rubric:: 范例
   .. code-block:: lua
      :caption: Lua:

         Take = reaper.MIDIEditor_GetTake(midieditor)





