# 洗衣机算法设计


        选择洗衣模式：水位，浸泡时间，漂洗次数；
        注水，到达一定水量停止 ；
        浸泡，计时 ；
        滚筒转动, 左3圈，右3圈 ；
        排水，排到最低水位 ；
        滚筒转动，脱水；
        结束；

        GET 选择模式
        water_in_switch(open)
        UNTILL 一定水量
        water_in_switch(close)
        浸泡
        UNTILL 到达浸泡时间
        for(次数=0;次数<规定次数；次数++)
        滚筒转动，左3圈，右3圈
        while(水位>最低水位)
        排水
        while(水位==最低水位)
        滚筒转动，脱水
        end while
        end;