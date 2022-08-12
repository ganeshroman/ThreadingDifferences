# Fragment & Activity

| Activity |  Fragment |
|----------|:---------:|
| Activity is an application component that gives a user interface where the user can interact. | The fragment is only part of an activity, it basically contributes its UI to that activity.|
| Activity is not dependent on fragment | 	Fragment is dependent on activity. It can’t exist independently. |
| we need to mention all activity it in the manifest.xml file | 	Fragment is not required to mention in  the manifest file |
| We can’t create multi-screen UI without using fragment in an activity, |	After using multiple fragments in a single activity, we can create a multi-screen UI.|
|Activity can exist without a Fragment |  	Fragment cannot be used without an Activity. |
| Creating a project using only Activity then it’s difficult to manage |	While Using fragments in the project, the project structure will be good and we can handle it easily. |
| Lifecycle methods are hosted by OS. The activity has its own life cycle. |	Lifecycle methods in fragments are hosted by hosting the activity. |
| Activity is not lite weight. | 	The fragment is the lite weight. |
