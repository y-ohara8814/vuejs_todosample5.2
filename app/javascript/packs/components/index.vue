<template>
  <div>
    <!-- 新規作成部分 -->
    <div class="row">
      <div class="col s10 m11">
        <input class="form-control" placeholder="Add your task!!">
      </div>
      <div class="col s2 m1">
        <div class="btn-floating waves-effect waves-light red">
          <i class="material-icons">add</i>
        </div>
      </div>
    </div>
    <!-- リスト表示部分 -->
    <div>
      <ul class="collection">
        <li id="row_task_1" class="collection-item">
            <label for="task_1">
                <input type="checkbox" id="task_1" />
                <span>Sample Task</span>
            </label>
        </li>
        <li id="row_task_2" class="collection-item">
            <label for="task_2">
                <input type="checkbox" id="task_2" />
                <span>Sample Task</span>
            </label>
        </li>
        <li id="row_task_3" class="collection-item">
            <label for="task_3">
                <input type="checkbox" id="task_3" />
                <span>Sample Task</span>
            </label>
        </li>
      </ul>
    </div>
    <!-- 完了済みタスク表示ボタン -->
    <div class="btn">Display finished tasks</div>
    <!-- 完了済みタスク一覧 -->
    <div id="finished-tasks" class="display_none">
      <ul class="collection">
        <li id="row_task_4" class="collection-item">
            <label v-bind:for="'task_4'">
                <input type="checkbox" v-bind:id="'task_4'" checked="checked"/>
                <span>Done Task</span>
            </label>
        </li>
        <li id="row_task_5" class="collection-item">
            <label v-bind:for="'task_5'">
                <input type="checkbox" v-bind:id="'task_5'" checked="checked"/>
                <span>Done Task</span>
            </label>
        </li>
      </ul>
    </div>
  </div>
</template>
