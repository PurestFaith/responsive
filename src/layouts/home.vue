<template>
  <div class="">
    <!-- 导航 -->
    <div
      class="sticky top-0 flex w-full items-center justify-between bg-green-600 p-5 shadow-lg"
    >
      <div class="font-semibold">
        <div>MY</div>
        <div>PERSONAL</div>
      </div>
      <div class="cursor-pointer md:hidden" @click="flag">开关</div>
      <div
        :class="{ hidden: isActive, flex: !isActive }"
        class="absolute left-0 right-0 top-5 translate-y-16 cursor-pointer flex-col items-center gap-4 bg-green-600 p-4 shadow-lg md:static md:flex md:translate-y-0 md:flex-row md:bg-opacity-0 md:bg-none md:shadow-none"
        role="menu"
        aria-expanded="false"
        ref="box"
      >
        <div class="mb-1 underline-offset-8 hover:underline md:ml-10">首页</div>
        <div class="mb-1 underline-offset-8 hover:underline md:ml-10">关于</div>
        <div class="mb-1 underline-offset-8 hover:underline md:ml-10">联系</div>
        <div class="mb-1 underline-offset-8 hover:underline md:ml-10">登录</div>
      </div>
    </div>

    <!-- 内容 -->
    <div class="mx-3 mt-3 md:flex md:justify-between 2xl:flex-wrap">
      <div
        class="mb-3 w-full rounded-lg bg-slate-400 p-3 md:mr-3 md:w-[500px] md:text-right 2xl:mr-0 2xl:w-full"
      >
        <div class="mb-2 font-[700]">MESSAGE</div>
        <div>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Culpa
          recusandae sit fugiat dolore maiores vitae optio veniam minus sed,
          accusamus labore assumenda praesentium atque et! Totam vel
          necessitatibus inventore sunt? Lorem ipsum dolor, sit amet consectetur
          adipisicing elit. Culentore sunt? Lorem ipsum dolor, sit amet
          consectetur adipisicing elit. Culpa recusandae sit fugiat dolore
          maiores vitae optio veniam minus sed, accusamus labore assumenda
          praesentium atque et! Totam vel necessitatibus inventore sunt?
        </div>
      </div>
      <div
        class="mb-3 w-full rounded-lg bg-rose-400 p-3 md:mr-3 md:w-[500px] md:text-right 2xl:mr-0 2xl:w-full"
      >
        <div class="mb-2 font-[700]">MESSAGE</div>
        <div>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Culpa
          recusandae sit fugiat dolore maiores vitae optio veniam minus sed,
          accusamus labore assumenda praesentium atque et! Totam vel
          necessitatibus inventore sunt? Lorem ipsum dolor, sit amet consectetur
          adipisicing elit. Culentore sunt? Lorem ipsum dolor, sit amet
          consectetur adipisicing elit. Culpa recusandae sit fugiat dolore
          maiores vitae optio veniam minus sed, accusamus labore assumenda
          praesentium atque et! Totam vel necessitatibus inventore sunt?
        </div>
      </div>
      <div
        class="mb-3 w-full rounded-lg bg-violet-600 p-3 md:mr-3 md:w-[500px] md:text-right"
      >
        <div class="mb-2 font-[700]">MESSAGE</div>
        <div>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Culpa
          recusandae sit fugiat dolore maiores vitae optio veniam minus sed,
          accusamus labore assumenda praesentium atque et! Totam vel
          necessitatibus inventore sunt?s labore assumenda praesentium atque et!
          Totam vel necessitatibus inventore re maiores vitae optio veniam minus
          sed, accusamus labore assumenda praesentium atq
        </div>
      </div>
      <div
        class="mb-3 w-full rounded-lg bg-amber-600 p-3 md:mr-3 md:w-[500px] md:text-right 2xl:mr-0"
      >
        <div class="mb-2 font-[700]">MESSAGE</div>
        <div>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Culpa
          recusandae sit fugiaesentium atque et! Totam vel necessitatibus
          inventore sunt?
        </div>
      </div>
      <div
        class="mb-3 w-full rounded-lg bg-emerald-600 p-3 md:w-[500px] md:text-right"
      >
        <div class="mb-2 font-[700]">MESSAGE</div>
        <div>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Culpa
          recusandae sit fugiat dolore maiores vitae optio veniam minus sed,
          accusamus labore assumenda praesentium atque et! Totam vel
          necessitatibus inventore sunt?t
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
const box = ref<HTMLDivElement | null>(null)
const isActive = ref(true)
const flag = () => {
  isActive.value = !isActive.value
}
</script>
