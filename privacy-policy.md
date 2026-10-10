pop-senpai-2 privacy policy
Effective date: October 9, 2026. This policy describes the current private alpha of pop-senpai-2.

Operator and requests
The operator can be contacted at INTJMuhant@gmail.com. Use this address to request access to, correction of, or deletion of bot-retained information. The operator handles requests through this contact. To remove all bot-retained state locally, stop the bot and delete its .local-data/application-state.dpapi file. Discord and the game service keep any data they retain under their own policies.

What the bot receives and uses
Discord sends message events for channels the bot can access and for direct messages to the bot. These events include author and channel metadata even when the author is not an approved operator. Without privileged Message Content intent, Discord generally supplies message content only for direct messages to the bot, messages mentioning it, and its own messages. The bot checks the configured owner/operator user-ID allowlist before processing a command and does not retain rejected messages. It disables discord.py's in-memory message cache. Error logs contain safe event categories and random correlation references; they do not contain message text, user IDs, tokens, exception text, or host paths.

For chat send, the bot receives the exact requested body and selected channel, home kingdom, and castle. It sends that body once through the configured local PNC operational facade, which uses the local game client. A send without a body opens a requester-bound entry form; the form keeps the requester and target in process memory until submission or expiration. No unsolicited direct messages are sent.

What the bot retains
The bot stores its application state in .local-data/application-state.dpapi, an ignored local file encrypted with Windows DPAPI for the current Windows user. It atomically replaces encrypted state, fails the current operation if encryption fails, and cannot start when existing state cannot be decrypted. It has no plaintext fallback. The current process still has the permissions of the signed-in Windows account, and DPAPI does not isolate data from other software running as that account.

The encrypted state retains:

configured Discord user IDs for connection bindings and send creators;
configured game account and instance identifiers, physical BlueStacks instance key, process ID, and exact process-creation time for each connection or send;
actor defaults and owner pause intent;
each send's Discord message or modal-interaction request ID, exact requested body, selected channel, kingdom and castle, typed outcome, submission evidence, and safe error code.
The journal exists to prevent duplicate request IDs from sending twice, preserve uncertain outcomes across restart, prevent a later receipt-equivalent message from falsely confirming an earlier unresolved send, and show saved status. The exact body is retained because it is part of the idempotency and ambiguity record. The bot does not display saved mpop-senpai privacy policy
Effective date: October 10, 2026.

This policy applies to the pop-senpai Discord bot. Its privacy commitments apply regardless of the game context, platform, or technical implementation used to carry out your requests.

Information used
The bot uses only information needed to authorize users and handle their requested commands:

Discord user, server, channel, and request identifiers;
command or form content you submit, including text you explicitly ask it to send;
selected game-context and target details, preferences, and operational session identifiers;
request status, timestamps, outcomes, and diagnostic information needed for reliability and support.
Discord may deliver message-event metadata from channels the bot can access. The bot accepts commands only from authorized users and does not retain rejected message content. It does not build personal profiles or request email addresses, friend lists, passwords, payment information, or other unrelated personal details. Do not submit passwords, tokens, financial details, health information, or other sensitive personal information in commands.

Purposes and commitments
Information is used to check access, carry out commands, maintain your selected game context, prevent duplicate or uncertain operations, and provide status and support. Submitted message text may be retained when necessary for these reliability protections.

We do not sell user information, use it for advertising or personal profiling, or use Discord data to train machine-learning models. The bot does not send unsolicited direct messages or upload images or screenshots to Discord. Routine bot diagnostics do not include human user IDs, command bodies, passwords, or tokens.

Sharing and visibility
Discord processes commands and replies as part of its service. Replies appear where you invoke the bot and may be visible to other people with access to that channel.

When you explicitly request an action that sends content to a selected game context or external service, that destination receives the information needed for the action. Connected services may also create local diagnostic records or captures containing the requested content. These operator-controlled copies are included in our security and deletion responsibilities. We do not share information for unrelated purposes; any other disclosure must be necessary to operate the service under appropriate safeguards or required by law.

Discord and external services control their own copies under their respective privacy policies. The operator cannot directly erase records controlled by those services.

Retention and security
Access settings, connection preferences, and request history are kept only for the purposes described above. Saved request history currently has no automatic expiry: the operator must remove it promptly when it is no longer needed, when a valid deletion request is received, or when the bot permanently stops operating, except where retention is legally required. Disconnecting a game context does not itself erase prior request history.

Primary saved connection and command records are encrypted. Access is restricted, and credentials are kept out of public replies and routine logs. Required security and deletion coverage for additional copies must be verified before enabling features that produce them. We will address security incidents and notify affected users and Discord as required.

Access, correction, and deletion
For support or to request access to, correction of, or deletion of information held by the operator, contact the operator. We may request only the information necessary to verify ownership and locate the relevant records. Requests cover bot records and related copies under the operator's control and will be handled promptly.

Changes
A change of game context or implementation does not remove these commitments. If a feature changes what personal data is used, its purpose, recipients, or retention, this policy must be updated before that feature is enabled, with notice of material changes. This policy does not replace Discord's applicable terms or policies.essage bodies through job list or job status. A creator can inspect their own send status; the configured owner can inspect all send statuses.

The bot keeps connection and send state until the local encrypted file is deleted. worker disconnect removes only the selected actor's connection binding and does not delete send history. The configured support address is the request route for access, correction, and deletion; local file deletion removes all bot-retained records. On permanent shutdown, the operator must promptly delete retained API data that is no longer needed. The local PNC workflow may separately retain UI evidence, screenshots, or game-chat archives containing the requested body in PNC's configured local data directory; the bot does not send artifact paths or screenshots to Discord. PNC writes these as ordinary files. Encryption at rest for these separate copies still needs deployment verification before live Discord-to-game sending, and deletion requests must cover them as well.

Sharing and services
Discord provides the Gateway and carries the incoming command, command author ID, and bot reply. The bot's chat command passes the requested body to the local PNC package and game client; the game service may receive it as part of normal game operation. The bot does not send command bodies to a separate hosted bot backend. The operator's Windows account, its configured PNC installation, Discord, and the game service are separate systems with their own access and retention controls.

Scope and changes
This policy describes help, local worker connection management for configured BlueStacks sessions, one-shot chat sending, and saved send status. It does not claim that Discord or game-publisher terms are fully satisfied. The operator must keep an accurate policy available at a public HTTPS address, configure that address in the bot settings and Developer Portal, and keep the support/deletion contact working. The operator should update this policy before adding any feature that retains other message content, chat transcripts, registrations, or generated outputs.
