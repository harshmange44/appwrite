import 'package:appwrite/appwrite.dart';

// Init SDK
Client client = Client();
Avatars avatars = Avatars(client);

client
    .setProject('5df5acd0d48c2') // Your project ID
;

String result = avatars.getCreditCard(
    code: 'amex',
);

print(result); // Resource URL string