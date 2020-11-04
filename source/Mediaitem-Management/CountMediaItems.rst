CountMediaItems
=============================================
.. raw:: html

    <span>
        提交者: noiZ&nbsp;&nbsp;&nbsp;&nbsp;提交日期: 2020-10-24
    </span>
    <p></p>
    
``CountMediaItems``\(*obj proj*)
   获取工程中的item数量

      :参数:
         **obj proj**
            工程对象，一般填0

      :返回:
            HWND

   .. note::
         一般用于确定循环遍历工程中所有item时的终点


         
   .. rubric:: 范例
   .. code-block:: c++
      :caption: C++:

         CountMediaItems(ReaProject* proj)

   .. code-block:: javascript
      :caption: EEL:

         CountMediaItems(ReaProject proj)

   .. code-block:: lua
      :caption: Lua:

         reaper.CountMediaItems(ReaProject proj)

   .. code-block:: python
      :caption: Python:

         RPR_CountMediaItems(ReaProject proj)


   .. rubric:: 更多范例
   .. code-block::

            local num=reaper.CountMediaItems(0)
            for i=0, num-1 do
                local item=reaper.GetMediaItem(0, i)
            end




