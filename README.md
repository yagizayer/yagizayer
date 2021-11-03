
<<<<<<< Updated upstream
### Hi there 👋 ssss
=======
<<<<<<< HEAD
### Hi there 👋aaaaa
=======
### Hi there 👋 ssss
>>>>>>> 7ef9f446e7b0e17737f65dc137d87d9ff9b857ee
>>>>>>> Stashed changes

<!--
**yagizayer/yagizayer** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:
-->

- 🔭 I’m currently working on Unity and Unreal Engine.
- 🌱 I’m currently learning well... basically everything i can.
- 💬 Ask me about anything, i will do my best to help :)
- 📫 How to reach me: [![GmailIcon](Resources/gmailIcon.png)](mailto:yagizayeryy@gmail.com)
- 😄 Pronouns: M'dude!
- ⚡ Fun fact: I can do this:</br> ![GooglyEyes](Resources/googlyEyes.png)

------------------------    Play My Games!    ------------------------ <br>
All of my games are open source<br>

Fps Reflex Enhancer : https://yagizayer.github.io/Fps_Reflex_Game_v03/<br>
Temple of Artemis : https://yagizayer.github.io/Temple-Of-Artemis/<br>
Health Racer : https://yagizayer.github.io/HealthRacer/<br>
Rollercoaster Simulator : https://yagizayer.github.io/RollerCoasterSimulator/<br>
Arcade 2D Game - Pizza Time  : https://yagizayer.github.io/PizzaTime_v01/<br>
I Wanna Become JEDI  : https://yagizayer.github.io/FireByteGames_Case_01/<br>

------------------------    yagizayer.cs    ------------------------*/<br>

    using System.Collections.Generic;
    using UnityEngine;
    
    [RequireComponent(typeof(DecentCoworkers), typeof(CozyEnvironment))]
    public class YagizAyer : MonoBehaviour
    {
    
        [Header("Contact Info")]
        public const string GithubAddress = "github.com/yagizayer";
        public const string EMailAddress = "yagizayeryy@gmail.com";
        public const string Phone = "+90 544 828 8564";
        public static (Country, City) CurrentAddress = (Country.Turkey, City.Mugla);
    
        [Tooltip("The field that Yagiz prefers to work in")]
        [SerializeField] private WorkArea _workingPreferences = WorkArea.GameMaking;
    
    
        [Tooltip("General working experience")] // TODO : Gain more experience
        private List<(DateRange, int, Company)> _workingExperience = new List<(DateRange, int, Company)>()
        {
            (
                DateRange.Month,
                3,
                new Company(
                    name: "GefeaSoft",
                    workingArea: WorkArea.Simulations,
                    location: City.Mugla,
                    website :"gefeasoft.com",
                    contact :new Contact(
                        "Gizem KAYAR",
                        Role.Manager
                    )
                )
            ),
            (
                DateRange.Year,
                1,
                new Company(
                    name: "Atolye45",
                    workingArea: WorkArea.WebFullStack,
                    location: City.Manisa,
                    website :"atolye45.com",
                    contact :new Contact(
                        "Emrah Vardaroğlu",
                        Role.Manager
                    )
                )
            ),
            (
                DateRange.Month,
                3,
                new Company(
                    name: "Freelance",
                    workingArea: WorkArea.GameMaking,
                    location: City.Remote,
                    website :"peopleperhour.com",
                    contact :new Contact(
                        "Heiko K.",
                        Role.Customer
                    )
                )
            )
        };
    
    
        [Tooltip("Birth information of Yagiz")]
        private Birth _birth = new Birth(
            country: Country.Turkey,
            city: City.Manisa,
            year: 1997
        );
    
    
        [Tooltip("Unity Experiences of Yagiz")]
        private List<(ExperienceLevel, string)> _unityExperiences = new List<(ExperienceLevel, string)>()
        {
            (ExperienceLevel.Intermediate,"Callbacks and UnityActions"),
            (ExperienceLevel.Intermediate,"Event Driven Programming"),
            (ExperienceLevel.Intermediate,"CleanCode Education"),
            (ExperienceLevel.Intermediate,"Scriptable Objects"),
            (ExperienceLevel.Intermediate,"Project Management"),
            (ExperienceLevel.Intermediate,"CineMachine"),
            (ExperienceLevel.BelowIntermediate,"Unity Collab"),
            (ExperienceLevel.BelowIntermediate,"Spline Tools"),
            (ExperienceLevel.BelowIntermediate,"Runtime Mesh Operations"),
        };
    
    
        [Tooltip("Blender Experiences of Yagiz")]
        private List<(ExperienceLevel, string)> _blenderExperiences = new List<(ExperienceLevel, string)>()
        {
            (ExperienceLevel.Intermediate,"Model Re-shaping"),
            (ExperienceLevel.BelowIntermediate,"Modifiers"),
            (ExperienceLevel.BelowIntermediate,"Texturing"),
            (ExperienceLevel.BelowIntermediate,"Material Operations"),
            (ExperienceLevel.BelowIntermediate,"Mesh Operations"),
        };
    
    
        [Tooltip("Other Experiences of Yagiz")]
        private List<(ExperienceLevel, string)> _otherExperiences = new List<(ExperienceLevel, string)>()
        {
            (ExperienceLevel.Intermediate,"Html-Css-Javascript"),
            (ExperienceLevel.Intermediate,"Php"),
            (ExperienceLevel.Intermediate,"Adobe xd"),
            (ExperienceLevel.BelowIntermediate,"Flutter"),
            (ExperienceLevel.BelowIntermediate,"Mongo Database"),
            (ExperienceLevel.BelowIntermediate,"Nodejs-Angular 6"),
        };
    
    
        [Tooltip("Education of Yagiz")]
        private Education _education = new Education(
            highSchool: (EducationState.Completed, "Manisa Anatolian Technical and Industrial Profession High School, Data Analysis Program"),
            bachelors: (EducationState.Completed, "Muğla Sıtkı Koçman University, Department of Information Systems Engineering"),
            masters: (EducationState.InProgress, "Muğla Sıtkı Koçman University, Department of Digital Game Design and Technologies"),
            phds: (EducationState.Hopeful, "?")
        );
    
        [Tooltip("Hobbies of Yagiz")]
        private List<(Occurrence, string)> _hobbies = new List<(Occurrence, string)>(){
            (Occurrence.Everyday, "Research about new games"),
            (Occurrence.Everyday, "Listening music while coding"),
            (Occurrence.FewTimesAWeek, "Playing Video games"),
            (Occurrence.OnceAWeek, "Socializing with friends"),
            (Occurrence.FewTimesAMonth, "Going to cinema"),
            (Occurrence.OnceAMonth, "Going to Hiking"),
            (Occurrence.OnceInAWhile, "Camping"),
        };
    
    
        [Tooltip("Goals of Yagiz")]
        [SerializeField]
        private List<(Goal, string)> _goals = new List<(Goal, string)>(){
            (Goal.ShortTerm, "Writing a game scenario in a month"),
            (Goal.ShortTerm, "Making at least 20 games by the end of 2021"),
            (Goal.ShortTerm, "Making at least 1 game with machine learning in 6 months"),
            (Goal.ShortTerm, "Making at least 3 games with multiplayer in 6 months"),
            (Goal.MidTerm, "To learn enough French to understand everyday conversations in a year."),
            (Goal.MidTerm, "Traveling at least 1 country completely in 18 months."),
            (Goal.LongTerm, "Leading my own gaming team in 5 years."),
            (Goal.LongTerm, "Making a game that everyone has heard of in 7 years.")
        };
    }
