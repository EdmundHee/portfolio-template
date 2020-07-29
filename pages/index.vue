<template>
  <div class="flex flex-col w-screen h-full">
    <!-- Your name, profile picture and contact -->
    <HeadWrapper
      name="Edmund Hee"
      title="Full Stack Developer"
      userImgURL="https://cdn4.iconfinder.com/data/icons/instagram-ui-twotone/48/Paul-18-512.png"
      phone="+0123456789"
      email="edmund@thelead.io"
    />
    <!-- About Me -->
    <AboutWrapper
      aboutMe="I'm a full stack web developer and self-taught Data Scientist"
      linkedInURL="https://www.linkedin.com/in/edmundhee/"
      languages="English, Chinese & Malay"
      nationality="Malaysian"
      interest="Coffee"
    />
    <!-- Working Experience -->
    <CareerWrapper>
      <template v-slot:career>
        <Career
          companyName="AirAsia"
          title="Data Scientist"
          startDate="Nov 2017"
          endDate="Nov 2019"
        >
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>Built Dashboard & Reports for Business Userse</li>
              <li>Built API Servers to support Web Application and Mobile Application</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
            </ul>
          </template>
        </Career>

        <Career
          companyName="SPNQ Software Hub"
          title="Full Stack Web Developer"
          startDate="July 2016"
          endDate="Nov 2017"
        >
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>Built Business Web Application for business users</li>
              <li>Created Data Warehouse solutions for the company</li>
              <li>Created single source of true for the client</li>
              <li>Created single source of true for the client</li>
              <li>Created single source of true for the client</li>
            </ul>
          </template>
        </Career>
      </template>
    </CareerWrapper>
    <!-- Achievement -->
    <AchievementWrapper project="15" client="15k" award="10"/>
    <!-- Portfolio -->
    <PortfolioWrapper>
      <template v-slot:portfolio>
        <div class="grid grid-cols-1 md:grid-cols-3">
          <ProjectCard
            imgUrl="../img/github.png"
            name="My own Portfolio"
            project="NuxtJS Project"
            projectURL="https://github.com/edmundhee/portfolio-template"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />
        </div>
      </template>
    </PortfolioWrapper>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "Edmund Hee | FullStack Developer"
    };
  }
};
</script>