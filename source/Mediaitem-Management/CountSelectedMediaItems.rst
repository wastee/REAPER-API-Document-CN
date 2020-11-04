CountSelectedMediaItems
=============================================
.. raw:: html

    <span>
        提交者: noiZ&nbsp;&nbsp;&nbsp;&nbsp;提交日期: 2020-10-24
    </span>
    <p></p>
    
``CountSelectedMediaItems``\(*obj proj*)
   获取选中的item数量

      :参数:
         **obj proj**
            工程对象，一般填0

      :返回:
            HWND

   .. note::
         一般用于确定循环遍历选中item时的终点


         
   .. rubric:: 范例
   .. code-block:: c++
      :caption: C++:

         CountSelectedMediaItems(ReaProject* proj)

   .. code-block:: javascript
      :caption: EEL:

         CountSelectedMediaItems(ReaProject proj)

   .. code-block:: lua
      :caption: Lua:

         reaper.CountSelectedMediaItems(ReaProject proj)

   .. code-block:: python
      :caption: Python:

         RPR_CountSelectedMediaItems(ReaProject proj)


   .. rubric:: 更多范例
   .. code-block::

            local num=reaper.CountSelectedMediaItems(0)
            for i=0, num-1 do
                local item=reaper.GetSelectedMediaItem(0, i)
            end




