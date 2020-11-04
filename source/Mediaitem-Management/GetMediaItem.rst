GetMediaItem
=============================================
.. raw:: html

    <span>
        提交者: noiZ&nbsp;&nbsp;&nbsp;&nbsp;提交日期: 2020-10-24
    </span>
    <p></p>
    
``GetMediaItem``\(*obj proj, int index*)
   通过序号获取获取工程中的item对象

      :参数:
         **obj proj**
            工程对象，一般填0
         **int index**
               工程中item的序号，以0为起点

      :返回:
            HWND

   .. note::
         Reaper中所有涉及到item次序的参数，均按照三个原则：

         #. 处于不同轨道的item，轨道编号小的item比大的顺序靠前

         #. 处于同一轨道的item，左边缘位置较小的顺序靠前

         #. 左边缘重叠的item，长度较大的顺序靠前

         

         如果用在循环遍历每一个item时，切勿在循环中做出任何会改变item序号的操作，包括改变位置、改变轨道、删除等等，因为序号是动态变化的，改变了一个序号往后的都同时变化。比如获取到0号item时把它删除，这样原来的1号item将会变成新的0号，后面的依次前移。这样原来的1号item就永远被跳过了，终点也会报错。正确的做法是在第一次遍历的时候，把每一个item对象存放到一个table里，遍历完成了再在table里循环并做各种操作。在已选中item中循环也同理。


         
   .. rubric:: 范例
   .. code-block:: c++
      :caption: C++:

         GetMediaItem(ReaProject* proj, int itemidx)

   .. code-block:: javascript
      :caption: EEL:

         GetMediaItem(ReaProject proj, int itemidx)

   .. code-block:: lua
      :caption: Lua:

         reaper.GetMediaItem(ReaProject proj, integer itemidx)

   .. code-block:: python
      :caption: Python:

         RPR_GetMediaItem(ReaProject proj, Int itemidx)





