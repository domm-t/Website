<template>
    <NuxtLayout>
        <section class="mx-auto space-y-8">
            <MiscLogoReveal />
            <!--<div class="flex flex-col items-center mx-auto mt-5">
                <MiscCountDown :time="1676053800000" />
            </div>-->
            <div
                class="max-w-7xl mx-auto mt-16 lg:mt-6 prose dark:prose-dark text-center p-2"
                data-aos="fade-up"
                data-aos-easing="linear"
                data-aos-delay="100"
                data-aos-duration="260"
            >
                A National Level technical symposium hosted by the department Electronics & Instrumentation of Easwari Engineering College.
            </div>

            <div
                class="flex flex-col items-center lg:justify-center gap-8 lg:flex-row mx-auto lg:mt-6 p-4"
            >
                <a
                    href="/pass"
                    data-aos="fade-up"
                    data-aos-easing="linear"
                    data-aos-delay="100"
                    data-aos-duration="260"
                    ><span class="sr-only">All Event Pass Register</span
                    ><ButtonTech size="120" text="All Pass Register" type="gray"
                /></a>
                <a
                    href="/register"
                    data-aos="fade-up"
                    data-aos-easing="linear"
                    data-aos-delay="100"
                    data-aos-duration="260"
                    ><span class="sr-only">Event Register</span
                    ><ButtonTech size="120" text="Event Register" type="gray"
                /></a>
            </div>
            <section class="lg:flex flex-1 w-full mx-auto mt-8 max-w-7xl">
                <div class="flex-1 w-full flex flex-col gap-8 items-center">
                    <div class="p-8">
                        <h1
                            class="text-center text-4xl font-bold font-atmospheric mx-auto"
                            data-aos="fade-up"
                            data-aos-easing="linear"
                            data-aos-delay="100"
                            data-aos-duration="260"
                        >
                            Technical Events
                        </h1>
                        <div
                            class="flex flex-row flex-wrap items-stretch justify-center gap-8 mt-6"
                        >
                            <a
                                v-for="event in technical"
                                :key="event._id"
                                :href="event._path"
                                class="flex flex-col gap-4 items-center w-full lg:max-w-xl p-8 border-2 border-zinc-700 dark:border-zinc bg-black/60 transition duration-500 ease-in-out transform hover:-translate-y-1"
                                data-aos="fade-up"
                                data-aos-easing="linear"
                                data-aos-delay="100"
                                data-aos-duration="260"
                            >
                                <div style="color:#18C0F1"
                                    class="uppercase text-base text- font-semibold text-center font-azonix"
                                >
                                   {{ event.title }}
                                </div>
                                <div class="text-lg text-center">
                                    {{ event.description }}
                                </div>
                            </a>
                        </div>
                    </div>
                    <div class="p-8">
                        <h1
                            class="text-center text-4xl font-bold font-atmospheric mx-auto"
                            data-aos="fade-up"
                            data-aos-easing="linear"
                            data-aos-delay="100"
                            data-aos-duration="260"
                        >
                            Non-Technical Events
                        </h1>
                        <div
                            class="flex flex-row flex-wrap items-stretch justify-center gap-8 mt-6"
                        >
                            <a
                                v-for="event in nonTechnical"
                                :key="event._id"
                                :href="event._path"
                                class="flex flex-col gap-4 items-center w-full lg:max-w-xl p-8 border-2 border-zinc-700 dark:border-zinc bg-black/60 transition duration-500 ease-in-out transform hover:-translate-y-1"
                                data-aos="fade-up"
                                data-aos-easing="linear"
                                data-aos-delay="100"
                                data-aos-duration="260"
                            >
                                <div style="color:#18C0F1"
                                    class="uppercase text-base font-semibold text-center font-azonix"
                                >
                                    {{ event.title }}
                                </div>
                                <div class="text-lg text-center">
                                    {{ event.description }}
                                </div>
                            </a>
                        </div>
                    </div>
                    <div class="p-8">
                        <h1
                            class="text-center text-4xl font-bold font-atmospheric mx-auto"
                            data-aos="fade-up"
                            data-aos-easing="linear"
                            data-aos-delay="100"
                            data-aos-duration="260"
                        >
                            Online Events
                        </h1>
                        <div
                            class="flex flex-row flex-wrap items-stretch justify-center gap-8 mt-6"
                        >
                            <a
                                v-for="event in onlineEvents"
                                :key="event._id"
                                :href="event._path"
                                class="flex flex-col gap-4 items-center w-full lg:max-w-xl p-8 border-2 border-zinc-700 dark:border-zinc bg-black/60 transition duration-500 ease-in-out transform hover:-translate-y-1"
                                data-aos="fade-up"
                                data-aos-easing="linear"
                                data-aos-delay="100"
                                data-aos-duration="260"
                            >
                                <div style="color:#18C0F1"
                                    class="uppercase text-base font-semibold text-center font-azonix" id="paper"
                                >
                                    {{ event.title }}
                                </div>
                                <div class="text-lg text-center">
                                    {{ event.description }}
                                </div>
                            </a>
                        </div>
                    </div>
                </div>
            </section>
            <div
                class="flex flex-col items-center gap-2 max-w-7xl mx-auto prose dark:prose-dark text-justify p-4"
                data-aos="fade-up"
                data-aos-easing="linear"
                data-aos-delay="100"
                data-aos-duration="260"
            >
                <h1
                    class="text-center text-4xl font-bold font-atmospheric mx-auto"
                    data-aos="fade-up"
                    data-aos-easing="linear"
                    data-aos-delay="100"
                    data-aos-duration="260"
                >
                    Contact
                </h1>
                <div
                    class="grid grid-cols-1 lg:grid-cols-2 font-azonix text-xl mx-auto"
                >
                    <div class="p-2">Vijay</div>
                    <a
                        class="p-2 block no-underline text-zinc-600 dark:text-royal-yellow"
                        href="tel:+919500163095"
                        >+91 73959 84868</a
                    >
                    <div class="p-2">Tamil</div>
                    <a
                        class="p-2 block no-underline text-zinc-600 dark:text-royal-yellow"
                        href="tel:+917550155076"
                        >+91 93601 12612</a
                    >
                </div>
            </div>
            <div
                class="flex flex-col lg:flex-row items-center gap-2 max-w-7xl mx-auto prose dark:prose-dark text-justify p-4"
                data-aos="fade-up"
                data-aos-easing="linear"
                data-aos-delay="100"
                data-aos-duration="260"
            >
                <img
                    src="/EEC_ICON.webp"
                    alt="Easwari Engineering College Logo"
                    class="w-48 mb-0"
                />
                <div class="p-2">
                    Easwari Engineering College is an educational institution
                    belonging to the SRM Group of Educational Institutions for
                    higher learning instituted in the academic year 1996 - 1997,
                    with the approval of Government of Tamil Nadu and AICTE. As
                    per government regulations for affiliation, the college was
                    initially affiliated to the University of Madras. The
                    college is now affiliated to Anna University Chennai since
                    2002. The college offers 11 UG programmes and 6 PG
                    programmes covering Engineering & Technology, and
                    Management.
                </div>
            </div>
            <div
                class="flex flex-col lg:flex-row-reverse items-center gap-2 max-w-7xl mx-auto prose dark:prose-dark text-justify p-4"
                data-aos="fade-up"
                data-aos-easing="linear"
                data-aos-delay="100"
                data-aos-duration="260"
            >
                

            </div>
        </section>
    </NuxtLayout>
</template>
<script setup lang="ts">
    useHead({
        title: "Instrublitz | Symposium",
        meta: [
            {
                name: "description",
                content:
                    "An annual tech festival hosted by the department of Electronics & Instrumentation of Easwari Engineering College.",
            },
        ],
    });
    const technical = await queryContent("events/technical-events").find();
    const nonTechnical = await queryContent(
        "events/non-technical-events"
    ).find();
    const onlineEvents = await queryContent("events/online-events").find();
</script>
