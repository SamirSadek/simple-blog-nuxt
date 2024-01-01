<template>
  <section
    class="flex flex-col-reverse md:flex-row md:h-96 w-4/5 mx-auto justify-between items-center"
  >
    <div class="container sm:mx-auto sm:p-32 p-4">
      <h2 class="text-Black font-bold text-5xl">
        Welcome to <span class="text-[#6C63FF]">DailyByte</span>
      </h2>
      <h2 class="text-black text-xl mt-4">
        Find the Best blog and explore others insights. Lorem ipsum dolor sit amet
        consectetur adipisicing elit. Perferendis voluptatum exercitationem tenetur
        consectetur blanditiis! Perferendis veritatis odio officiis!
      </h2>
      <div class="">
        <button
          class="right-0 mt-4 py-2 px-4 rounded-2xl bg-[#6C63FF] text-white font-bold"
        >
          <NuxtLink to="/"> Get Started </NuxtLink>
        </button>
      </div>
    </div>
    <div>
      <img src="/banner.png" alt="" />
    </div>
  </section>
</template>
