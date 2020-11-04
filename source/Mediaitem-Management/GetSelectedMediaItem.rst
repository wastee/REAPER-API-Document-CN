GetSelectedMediaItem
=============================================
.. raw:: html

    <span>
        提交者: noiZ&nbsp;&nbsp;&nbsp;&nbsp;提交日期: 2020-10-22
    </span>
    <p></p>
    
``GetSelectedMediaItem``\(*proj, index*)
   通过序号获取已选中的一个item对象

      :参数:
         **proj**
            工程对象，一般填0
         **index**
               被选中item的序号，以0为起点

      :返回:
            HWND

   .. note::
         Reaper中所有涉及到item次序的参数，均按照三个原则：

         #. 处于不同轨道的item，轨道编号小的item比大的顺序靠前

         #. 处于同一轨道的item，左边缘位置较小的顺序靠前

         #. 左边缘重叠的item，长度较大的顺序靠前


         
   .. rubric:: 范例
   .. code-block:: lua
      :caption: Lua:

         local item=reaper.GetSelectedMediaItem(0, 0)





