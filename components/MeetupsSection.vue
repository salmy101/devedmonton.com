<template>
    <div
        class="relative bg-white pt-8 -mt-8 pb-16 px-4 sm:px-6 lg:pt-12 lg:px-8"
    >
        <a id="meetups" href="/#meetups" class="anchor"></a>
        <div class="absolute inset-0">
            <div class="h-1/3 sm:h-2/3"></div>
        </div>
        <div class="relative max-w-7xl mx-auto">
            <div class="text-center">
                <h2
                    class="text-3xl leading-9 tracking-tight font-extrabold text-gray-900 sm:text-4xl sm:leading-10"
                >
                    Meetups We Support
                </h2>
            </div>
            <div
                class="mt-8 rounded-lg bg-gray-200 overflow-hidden shadow divide-y divide-gray-200 sm:divide-y-0 sm:grid sm:grid-cols-2 sm:gap-px"
            >
                <MeetupCard
                    :name="meetups.ruby.name"
                    :logo="meetups.ruby.logo"
                    :link-to="meetups.ruby.linkTo"
                    :slack-link="meetups.ruby.slackLink"
                    :slack="meetups.ruby.slack"
                >
                    <span>
                        YEGRB is Edmonton’s local Ruby Meetup. Ruby is a
                        dynamic, open source programming language with a focus
                        on simplicity and productivity. It has an elegant syntax
                        that is natural to read and easy to write.
                    </span>
                </MeetupCard>
                <MeetupCard
                    :name="meetups.javascript.name"
                    :logo="meetups.javascript.logo"
                    :link-to="meetups.javascript.linkTo"
                    :slack-link="meetups.javascript.slackLink"
                    :slack="meetups.javascript.slack"
                >
                    <span>
                        Exchange.js is an open community of local developers and
                        designers, who meet monthly to discuss a wide range of
                        topics within the JavaScript ecosystem.
                    </span>
                </MeetupCard>
                <MeetupCard
                    :name="meetups.edmontonPy.name"
                    :logo="meetups.edmontonPy.logo"
                    :link-to="meetups.edmontonPy.linkTo"
                    :slack-link="meetups.edmontonPy.slackLink"
                    :slack="meetups.edmontonPy.slack"
                >
                    <span>
                        We hope to foster a strong, supportive, and proficient
                        Python community in the Edmonton area. Everyone
                        interested in any aspect of Python development is
                        welcome to join.
                    </span>
                </MeetupCard>
                <MeetupCard
                    :name="meetups.dotNet.name"
                    :logo="meetups.dotNet.logo"
                    :link-to="meetups.dotNet.linkTo"
                    :slack-link="meetups.dotNet.slackLink"
                    :slack="meetups.dotNet.slack"
                >
                    <span>
                        The Edmonton .NET User Group is a non-profit
                        organization which empowers the IT Professionals and
                        Developers using the Microsoft .NET Framework.
                    </span>
                </MeetupCard>
                <!-- Cog svg icon provided by FontAwesome https://fontawesome.com/license/free -->
                <MeetupCard
                    :name="meetups.yegRug.name"
                    :logo="meetups.yegRug.logo"
                    :link-to="meetups.yegRug.linkTo"
                    :slack="meetups.yegRug.slack"
                    :slack-link="meetups.yegRug.slackLink"
                    logo-bg="bg-blue-100"
                >
                    <span>
                        The Edmonton R User Group (YEGRUG) is an R-enthusiast
                        group hosting events on data wrangling to visualization
                        and web development with R. Learn R, hone your skills,
                        network, all skill levels are welcome.
                    </span>
                </MeetupCard>
                <MeetupCard
                    :name="meetups.yegwit.name"
                    :logo="meetups.yegwit.logo"
                    :link-to="meetups.yegwit.linkTo"
                    :slack-link="meetups.yegwit.slackLink"
                    logo-bg="bg-blue-100"
                >
                    <span>
                        YEGWIT aims to build a strong and safe group for women,
                        diverse genders, and allies in tech with the goal of
                        fostering engagement and opportunity, providing
                        mentorship, and creating community. We are establishing
                        a group that allows individuals to share ideas,
                        concerns, thoughts and actions, to create an equitable
                        environment within the industry.
                    </span>
                </MeetupCard>
                <MeetupCard
                    :name="meetups.weeklydevchat.name"
                    :logo="meetups.weeklydevchat.logo"
                    :link-to="meetups.weeklydevchat.linkTo"
                >
                    <span>
                        Weekly Dev Chat is a place to ask questions, hear
                        different view points, and get to know your fellow
                        developers. Every week there is an initial topic posted
                        to get the discussion started. Sometimes we discuss the
                        initial topic the entire chat, other times the topic
                        changes several times through the natural flow of the
                        conversation. Everyone and anyone is welcome to join as
                        long as you are kind, supportive, and respectful of
                        others.
                    </span>
                </MeetupCard>
            </div>
        </div>
    </div>
</template>

<script>
import MeetupCard from "./MeetupCard.vue";

export default {
    components: { MeetupCard },
    data() {
        return {
            meetups: {
                ruby: {
                    name: "YEGrb",
                    logo: require("../assets/logos/ruby-240px.png"),
                    linkTo: "https://yegrb.com/",
                    slack: "#meetup-ruby",
                },
                javascript: {
                    name: "Exchange.js",
                    logo: require("../assets/logos/JavaScript-logo-240px.png"),
                    linkTo: "https://exchangejs.com/",
                    slack: "#meetup-javascript",
                },
                edmontonPy: {
                    name: "Edmonton.Py",
                    logo: require("../assets/logos/python-logo.svg"),
                    linkTo: "http://edmontonpy.com/",
                    slack: "#meetup-edmontonpy",
                },
                dotNet: {
                    name: "Edmonton .NET User Group",
                    logo: require("../assets/logos/dotNet_logo.png"),
                    linkTo: "http://edmug.net/",
                    slack: "#meetup-dotnet-edmug",
                },
                yegRug: {
                    name: "Edmonton R User Group",
                    logo: require("../assets/logos/r-logo.svg"),
                    linkTo:
                        "https://www.meetup.com/edmonton-r-user-group-yegrug",
                    slack: "#meetup-r",
                },
                yegwit: {
                    name: "Edmonton Women In Tech",
                    logo: require("../assets/logos/yegwit.png"),
                    linkTo: "https://yegwit.com/",
                    slack: "#meetup-r",
                },
                weeklydevchat: {
                    name: "Weekly Dev Chat",
                    logo: require("../assets/logos/weeklydevchat-logo.svg"),
                    linkTo: "https://weeklydevchat.com/",
                },
            },
        };
    },
};
</script>

<style></style>
