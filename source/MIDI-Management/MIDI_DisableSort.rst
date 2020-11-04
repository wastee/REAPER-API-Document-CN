MIDI_DisableSort
=============================================
.. raw:: html

    <span>
        提交者: 当归蛋&nbsp;&nbsp;&nbsp;&nbsp;提交日期: 2020-10-22
    </span>
    <p></p>
    
``MIDI_DisableSort``\(*MediaItem_Take*)
   对所有MIDI insert、delete、get和set函数禁用排序，直到调用MIDI\U Sort。

      :参数:
         **MediaItem_Take**
            需要提供当前处理的Take信息。

      :返回:
            窗口实例

   .. note::
         对于大量的MIDI数据处理，需要先启动这个API，然后再做处理，要不大量数据下的脚本运行速度极慢，动作完毕以后记得运行MIDI_Sort进行排序，不然会出现一些奇怪的问题。

         另外可以利用这个功能，对新插入的数据进行定位，比如CC数量是100，那么新插入的CC如果没有手动排序的话，ID就是101。


         
   .. rubric:: 范例





