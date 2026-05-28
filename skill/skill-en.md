# skill\-en\.md

## Meta Info

- **name**: fullstack\-pro\-engineering\-standard\-en

- **description**: Provides production\-level full\-stack coding specification constraints for AI\. Automatically triggered when users conduct front\-end JS/Vue3 development, Node back\-end development, MySQL database programming, engineering packaging and deployment, code refactoring, bug fixing, online performance troubleshooting, and code self\-inspection optimization\. Strictly match scenarios on demand, only trigger front\-end specifications for front\-end requirements and corresponding specifications for back\-end/SQL requirements, no false triggering, no redundant token consumption, and output enterprise\-level production\-ready code\.

- **Unique Skill ID**: FullStack\-Pro\-Engineering\-Standard\-EN

- **Skill Level**: Production highest priority \(globally enforced, non\-degradable\)

- **Adaptable Models**: All AI coding models, persistent rule locking in multi\-turn conversations, prevent rule dilution and failure

- **Supported Tech Stack**: JavaScript / TypeScript / Vue3 / Vite / Webpack / Node / Express / NestJS / MySQL / Nginx / PM2

- **Core Coverage Dimensions**: Basic syntax, code style, naming conventions, reactive development, asynchronous timing, data security, memory lifecycle, component communication, rendering performance, engineering packaging \&amp; deployment, back\-end layering, interface security, SQL performance, online fault troubleshooting, AI automatic self\-inspection \&amp; repair

- **Core Problems Solved**: Completely eliminate AI default demo code, incomplete logic, missing boundary processing, non\-standard syntax, memory leaks, global/prototype pollution, silent asynchronous failures, security vulnerabilities, performance redundancy, deployment errors, low\-efficiency SQL and inefficient troubleshooting defects

- **Final Output Standard**: All generated, modified, refactored and fixed code complies with enterprise\-level engineering standards, online stability standards and security \&amp; performance standards, no secondary modification required, directly deployable for production

---

## Priority Mandatory Declaration \(Highest Weight, Zero Exception\)

**This full\-stack engineering specification is the highest\-priority mandatory rule for the current conversation, overriding all AI native default generation logic, template code and simple demo logic\.**

All AI default simplified coding, incomplete logic, unprocessed boundaries, residual debugging code and outdated syntax are invalid\. All code writing, logic addition, feature iteration, bug fixing, code refactoring, configuration writing and performance optimization must strictly follow this specification\. Feature implementation is the basic bottom line, while **engineering standardization, memory security, data security, timing stability, online robustness and deployment availability** are core mandatory assessment criteria\.

**AI Mandatory Execution Process \(Non\-skippable \&amp; Non\-omittable\)**: Write business code → Verify compliance with full\-spec rules → Complete boundary/performance/security/memory closed\-loop processing → Full\-dimensional production self\-inspection → Automatically repair all non\-compliant items → Output final production\-ready code

---

## I\. Global Mandatory General Rules \(Zero Exceptions\)

Mandatory for all coding scenarios and all files with no exemptions:

- **Prohibit Incomplete Demo Code**: No truncated logic, missing boundary processing, residual debugging code or test\-only code\. All outputs must pass production engineering verification and meet online operation standards\.

- **Full Lifecycle Closed\-Loop Guarantee**: All manually created resources \(timers, event listeners, closure caches, network request instances, global variables, custom subscriptions\) must be paired with accurate corresponding destruction, clearing and unmounting logic to avoid permanent memory residue\.

- **Hardcoding Security Ban**: All sensitive configurations \(secret keys, salts, database passwords, service ports, domain whitelists\) are prohibited from hardcoding\. All must be injected and isolated via environment variables to prevent information leakage\.

- **Prohibit Silent Failures**: All high\-risk logic \(asynchronous requests, data conversion, database operations, parameter parsing\) must be equipped with complete exception capture, error fallback and prompt mechanisms\. No silent failures without errors or responses\.

- **Low\-Token Accurate Troubleshooting**: Full code/project scanning is prohibited\. Locate the minimum faulty code snippet based on error phenomena, analyze, locate and fix problems targeted only, avoid redundant token consumption and invalid analysis\.

- **Long Conversation Rule Lock**: Persist in specification standards when context is diluted in multi\-turn conversations, prohibit regression to AI default template generation logic and code degradation\.

- **Code Style \&amp; Directory Standards**: Follow unified naming rules strictly: PascalCase for components, camelCase for functions/variables, kebab\-case for file directories\. No case confusion or random naming\. Reuse existing project directory structure and prohibit messy custom directories\.

- **Single Responsibility \&amp; Code Line Constraint**: Prohibit oversized messy functions\. A single business function shall not exceed 20 lines\. One function handles only one responsibility; complex logic must be split into sub\-functions/utils to avoid bloated code\.

- **Reuse Priority Principle**: Prioritize existing project utilities, components, public methods and request encapsulations before writing new code\. Prohibit repeated wheel creation and redundant encapsulation\.

- **TypeScript Strict Type Constraint**: Explicit types/Interfaces must be defined for all variables, function inputs and outputs, and interface data\. Prohibit arbitrary any, ambiguous types and type escape\. Complex business types must be extracted into independent type files\.

- **Git Commit Specification**: All commits follow unified rules \(feat/fix/docs/style/refactor/test/chore\)\. No meaningless or mixed batch commits\. A single commit only handles one business or one fix to ensure traceability and rollback capability\.

- **Code Comment Mandatory Rules**: Complex business logic, special algorithms, boundary processing and third\-party adaptation logic require business comments\. Public utility functions require function, input and output descriptions\. Prohibit redundant useless comments and expired residual comments\.

- **Unified Error Code \&amp; Response Standard**: All interfaces and exceptions must use project\-unified error codes and prompt texts\. Prohibit random custom error texts and inconsistent return formats\. Distinguish client errors, server errors, permission errors and parameter errors for standardized output\.

- **Cross\-Origin Specification**: Business cross\-origin must adopt back\-end whitelist configuration\. Prohibit temporary front\-end cross\-origin fallback and global full\-domain cross\-origin allowance\. Unified local development proxy configuration; disable proxy penetration in production to avoid security vulnerabilities\.

- **Data Caching Specification**: Local cache \(localStorage/sessionStorage\) only stores non\-sensitive configuration and display data\. Prohibit plaintext storage of tokens and user privacy data\. All caches must have expiration strategies to prevent permanent dirty data; update cache synchronously with data changes\.

- **Browser Compatibility Specification**: Prohibit deprecated APIs and syntax\. Prioritize compatible syntax; provide downgrade fallback if new features are used\. Adapt to mainstream modern browsers to avoid online functional failures on low\-version browsers or partial devices\.

---

## II\. JavaScript Enterprise\-Level Coding Specification

All JS/TS business logic, utility functions, data processing, asynchronous logic and lifecycle logic must strictly comply with this production\-level mandatory specification\. Unify code styles, eliminate low\-level syntax bugs, prevent data pollution and memory leaks, solve silent asynchronous failures and timing chaos, and ensure all output code meets production stability standards\.

- **1\. Basic Syntax Mandatory Rules \(Eliminate Low\-Level Bugs\)**: Use `const / let` exclusively for variable declaration, completely abandon `var` to avoid variable hoisting, temporal dead zone, global pollution and duplicate declaration issues\.

- Use strict equality `=== / \!==` for all condition judgments and value comparisons; prohibit `== / \!=` to eliminate logic exceptions caused by implicit type conversion\.

- All variables must be explicitly declared before use; prohibit undeclared assignment to avoid implicit global mounting and hidden pollution\.

- Adopt standard ES6\+ syntax exclusively; prohibit deprecated APIs, obsolete events and outdated compatible writing to ensure modernization and maintainability\.

- **2\. Global \&amp; Prototype Security Rules \(Prevent Pollution \&amp; Conflict\)**: Strictly prohibit modification, rewriting and extension of native constructors such as Object, Array, String, Number and Function to avoid prototype pollution risks\.

- All public utilities must be independently encapsulated in dedicated modules; prohibit mounting to native prototypes to prevent global logic conflicts and overrides\.

- Prohibit random mounting of window/global variables; global states are uniformly managed via state management or public modules to control global variable proliferation\.

- **3\. This Context Binding Rules \(Unified Execution Context\)**: Use regular functions for scenarios requiring dynamic this binding \(DOM event callbacks, timer business logic, object method calls\)\.

- Use arrow functions only for scenarios inheriting outer context without dynamic this binding; prohibit random mixed usage without reason\.

- **4\. Asynchronous Programming Standardization \(Fix Silent Asynchronous Bugs\)**: Select Promise methods accurately, prohibit blind abuse: use `Promise\.all` for full\-success required tasks; use `Promise\.allSettled` for partial failure tolerant tasks; use `Promise\.race` for timeout interception and race condition handling\.

- Execute independent parallel requests in parallel; only use serial await for logically dependent requests, prohibit meaningless serial stacking and increased request latency\.

- Implement concurrency limiting for batch asynchronous tasks; prohibit unlimited batch requests to avoid browser queue blocking, page freezing and platform interface rate limiting\.

- All Promise and async/await logic must be equipped with complete catch exception handling and business fallback to eliminate silent asynchronous failures without logs or prompts\.

- **5\. Data Processing Rules \(Prevent Mutation \&amp; Rendering Errors\)**: **Data Copy Rules**: Use shallow copy for simple flat data; use deep copy for nested objects, multi\-level forms, tree structures and editable echo data\. Prohibit JSON serialization copy for complex data containing functions or regex to avoid data loss\.

- **Array Operation Rules**: Use map/filter/reduce/for\.\.\.of for read\-only traversal, mapping and filtering\. Copy first before modifying array data, prohibit direct original array mutation\. Prohibit arbitrary modification of array length or indexes to avoid implicit data mutation, reactive failure and abnormal business data\.

- **Special Data Structure Rules**: Use dedicated traversal methods for Set and Map; prohibit forced application of ordinary array methods to prevent data loss and value errors\.

- **Null \&amp; Numeric Fallback Rules**: Add null judgment and fallback for nested objects and uncertain interface data\. Intercept `NaN` and `Infinity` in all numeric calculations to avoid page blank and rendering crashes\.

- **Nullish Coalescence Rules**: Use `??` for business default value fallback; prohibit abuse of `\|\|` to avoid overwriting valid empty values such as 0, false and empty strings causing logic misjudgment\.

- **6\. Utility Function General Rules \(High Reusability \&amp; Fault Tolerance\)**: Follow single responsibility principle strictly, prohibit oversized messy functions\. Split complex business logic into independent sub\-functions and utilities\.

- All public utilities must have default input parameters and fault tolerance processing, no dependence on complete external parameters to avoid missing parameter errors\.

- Debounce and throttle utilities must have built\-in cancel reset and destruction capabilities\. Clear and reset high\-frequency event logic in component unmount phase to prevent residual execution and memory accumulation\.

- **7\. Memory \&amp; Closure Lifecycle Rules \(Eliminate Memory Leaks\)**: Prohibit multi\-layer closure nesting and closure nesting with timers/asynchronous logic to avoid variable capture disorder, occasional timing bugs and long\-term memory retention\.

- All timers, delayers, native event listeners, pending asynchronous requests and custom subscriptions must be fully cleared, unbound and destroyed to achieve complete lifecycle closed\-loop without zombie logic residue\.

- **8\. Unified Business Rules \(Global Style Consistency \&amp; Maintainability\)**: Prohibit scattered custom timestamps, date formats and manual time calculations\. Uniformly use public project utilities for time calculation and formatting to ensure global consistency\.

- Write clear business comments for complex logic, boundary processing, special compatibility and custom algorithms\. Update comments synchronously with code changes, prohibit expired and redundant useless comments\.

---

## III\. Vue3 Production\-Level Mandatory Specification

- **1\. Reactive Core Rules \(Prevent Reactive Failure\)**: Use `ref` for primitive types \(string/number/boolean\), use `reactive` for complex nested objects and arrays\. Prohibit mismatched scenario usage\.

- Prohibit direct destructuring of raw `reactive` objects; use `toRefs` for destructuring to retain complete reactivity\.

- Prohibit overall reassignment of `reactive` objects which will destroy reactive links\. Update data via `Object\.assign` or incremental field modification only\.

- **2\. Rendering \&amp; List Performance Rules \(Prevent Stuttering \&amp; Rendering Errors\)**: Distinguish instruction scenarios strictly: use`v\-show` for high\-frequency toggling components \(modals/dropdowns/tooltips\); use `v\-if` for low\-frequency display, permission control and components requiring destroy \&amp; rebuild\. Prohibit scenario reversal\.

- Prohibit array index as key in list rendering; use unique business IDs returned by backend to avoid DOM Diff reuse errors and data rendering overlap\.

- Enable virtual list, lazy loading and scroll throttling for long lists with data volume ≥ 1000 items\. Prohibit one\-time full rendering causing page stuttering and memory spikes\.

- **3\. Component Communication Standardization \(Unified Interaction\)**: Prohibit shorthand Props mode\. Fully configure Props with type verification, required status, default value and custom validation rules to eliminate implicit page exceptions caused by irregular parameter passing\.

- All custom component events must be explicitly declared via `emits`; prohibit random implicit event dispatch to ensure traceable and maintainable component communication\.

- **4\. Computed \&amp; Watch Rules \(Pure \&amp; Side\-Effect\-Free\)**: Computed must be pure read\-only functions without side effects\. Prohibit internal asynchronous requests and external data modification; use watch for asynchronous derivation logic\.

- Configure Watch accurately: enable `deep` for nested object/array monitoring; enable `immediate` for initial page execution needs\. Component internal watches are automatically unbound with component destruction, prohibit permanent residual monitoring\.

- **5\. Page Architecture Engineering Rules \(High Cohesion \&amp; Low Coupling\)**: Split complex page business logic into modular Composables to avoid bloated single\-file components and poor maintainability\.

- **6\. Full Lifecycle Closed\-Loop Rules \(Including KeepAlive Exclusive Solution, Eliminate Memory Leaks\)**: All resources created during component mounting must be completely cleared and destroyed on unmount to eliminate zombie logic and background residue\.

- Save timer/delayer instance IDs uniformly and clear them in `onUnmounted`\. Cancel all pending network requests on component unmount, prohibit asynchronous callbacks from modifying destroyed component states\.

- Unbind and remove all native event listeners, custom event subscriptions and global event mounts on component unmount to prevent event accumulation and repeated triggering\.

- Long\-term logic such as polling, heartbeat and scheduled refresh must be equipped with shutdown switches and terminated immediately when exiting the page\.

- Destroy third\-party instances \(charts/maps/rich text/players\) actively via official destroy methods on component unmount to release heap memory\.

- Prohibit DOM query, modification, state update and popup prompts after component unmount and DOM destruction\.

- **KeepAlive Exclusive Production Rules**: Do not rely solely on `onUnmounted` for cleanup, as cached components will not trigger this hook and cause permanent memory leaks\.

- Adopt **Dual Destruction Strategy** for cached components: clean timers, requests, listeners and side effects in both `onDeactivated` and `onUnmounted`\.

- Pause background persistent logic such as polling and real\-time subscription when cached components are deactivated to avoid silent resource consumption\.

- Reset loading status, clear expired request context and refresh old cache data when cached components are reactivated to prevent outdated logic and status display\.

- Prohibit components with frequent timing operations and real\-time subscriptions from being added to KeepAlive whitelist to avoid long\-term background risks\.

---

## IV\. Engineering, Packaging \&amp; Deployment Production Specification

- **Environment Isolation**: Completely independent configurations for development and production environments, prohibit mixed configuration and one\-size\-fits\-all global configuration\.

- **Production Mandatory Enable**: Code compression, Tree\-shaking, Gzip compression, route lazy loading, third\-party dependency chunk splitting, static resource CDN mapping\.

- **Production Mandatory Disable**: sourceMap, all console logs, debugger, hot update service and redundant debugging code\. Hot update resident is strictly prohibited in production\.

- **Nginx Production Standard**: Configure history mode 404 fallback, static resource hierarchical cache, Gzip compression and OPTIONS preflight release\. Prohibit global wildcard cross\-origin configuration to avoid security risks\.

- **PM2 Production Standard**: Enable process daemon, automatic exception restart, log segmentation and boot auto\-start\. Store sensitive configurations in environment variables, prohibit hardcoding and root user startup\.

- **Static Resource Cache Rules \(Fix Version Update Issues\)**: Add hash fingerprints to JS/CSS/image static resources for long\-term cache\. Disable strong cache for entry HTML and enable negotiated cache to solve user old version cache problems\.

- **Cross\-Origin Preflight Rules**: Configure reasonable OPTIONS preflight cache duration in production to avoid repeated invalid preflight requests\. Prohibit unrestricted global header and domain release\.

- **Package Volume Optimization Rules**: Eliminate unused dependencies, test code and mock code in production packaging\. Split large third\-party libraries independently to avoid oversized main bundle and slow first\-screen loading\.

- **Deployment Path Verification Rules**: Distinguish packaging static resource paths and CDN paths by environment, prohibit residual development environment paths causing production 404 errors\.

---

## V\. Node/Express/NestJS Backend Mandatory Specification

- **Express Basic Rules**: Mount parameter parsing, URL encoding parsing, domain whitelist cross\-origin and global exception middleware on service startup\. Prohibit bare interfaces without fallback processing\.

- **NestJS Layered Rules**: Controller is only responsible for route distribution and parameter reception\. All business logic, data calculation and database operations must be placed in Service layer, strictly prohibit layer confusion\.

- **Input Parameter Verification**: Verify all interface request parameters via Pipe for type, non\-null, format and range constraints\. Prohibit invalid parameters from entering business logic and database\.

- **Global Unified Capabilities**: Register global exception filters, response interceptors and permission guards uniformly, unify interface return formats, error codes and log specifications\.

- **JWT Security Rules**: Store keys and salts in environment variables, prohibit hardcoding\. Keep only minimal non\-sensitive fields in token payload\. Implement short\-term accessToken \+ long\-term refreshToken silent refresh \+ Redis blacklist instant invalidation mechanism\.

- **Request/Response Object Rules**: Prohibit global caching and reuse of req/res objects\. Each request lifecycle is independent to avoid request confusion, parameter pollution and memory accumulation\.

- **Interface Timeout Protection**: Configure unified timeout duration for all business interfaces, terminate logic and release connections automatically on timeout to prevent request hanging and connection pool exhaustion\.

- **Log Desensitization Mandatory**: Desensitize all interface and error logs\. Prohibit printing passwords, tokens, phone numbers, IDs and private data to prevent log leakage\.

- **Error Message Security Rules**: Prohibit returning native error stacks and database error information to the front end\. Encapsulate unified business prompts to prevent architecture, path and library information leakage\.

- **Request Body Rate Limiting**: Limit the maximum request body size uniformly, prohibit oversized malicious data packet attacks to prevent service memory overflow\.

- **Batch Operation Protection**: Add transactions and quantity limits for batch add/update/delete operations\. Prohibit unlimited batch operations causing database lag and table locking\.

---

## VI\. MySQL/SQL Security \&amp; Performance Specification

- **SQL Injection Prevention**: Prohibit manual splicing of user input parameters, use ORM parameterized queries exclusively to eliminate injection risks fundamentally\.

- **Index Validity Guarantee**: Prohibit function operations, implicit type conversion and prefix fuzzy matching on indexed fields\. Follow leftmost prefix principle strictly for composite indexes to ensure permanent index effectiveness\.

- **Data Consistency Guarantee**: Enable database transactions for core businesses such as multi\-table linkage modification, fund transactions and status synchronization to ensure atomicity \(all success or full rollback\)\.

- **Query Performance Optimization**: Prohibit `SELECT \*`, query required fields only to reduce disk IO and memory usage\.

- **Row Lock Anti\-Stuck Rules**: Prohibit abuse of `SELECT \.\.\. FOR UPDATE` pessimistic locks\. Avoid table locking and deadlocks caused by large transactions in non\-core transaction scenarios\.

- **Pagination Performance Rules**: Prohibit large offset deep pagination\. Use primary key backtracking pagination for deep queries to prevent full table scanning and performance collapse\.

- **Sort Index Rules**: Create indexes for business sorting fields\. Prohibit large table ORDER BY without indexes to avoid file sorting and temporary table query timeout\.

- **IN Query Quantity Limit**: Prohibit excessive parameters in IN statements\. Split batch queries for excessive parameters to prevent index failure and full table scanning\.

- **Large Field Query Isolation**: Prohibit loading TEXT/BLOB large fields in conventional list queries\. Query separately on demand to avoid excessive single data size and high IO dragging overall interface performance\.

- **Prohibit Nested Transactions**: Strictly prohibit multi\-layer nested transactions to prevent commit/rollback disorder, database deadlocks and data inconsistency\.

---

## VII\. Production\-Level Accurate Troubleshooting Mechanism \(Low\-Token \&amp; High\-Precision\)

This chapter is dedicated to online fault troubleshooting, abandoning AI default full\-scan inefficient mode\. Adopt full\-stack front\-end/back\-end/database/deployment fault experience to lock the minimum faulty code snippet based on phenomena, achieving low token consumption, accurate positioning and thorough repair for all production environment problems\.

- **Memory Leak Special Inspection**: Accurately check four core residual problems: uncleared timers/delayers, unbound native/custom event listeners, persistent closure references, undestroyed global variables/request instances\. Focus on KeepAlive dual destruction logic integrity\.

- **Rendering \&amp; Performance Inspection**: Target page stuttering, rendering disorder, white screen and data overlay problems\. Verify list key validity, v\-if/v\-show misuse, reactive assignment failure, direct array mutation, missing long\-list virtualization optimization and residual invalid DOM operations\.

- **Asynchronous Timing Inspection**: Solve silent asynchronous failures, timing disorder and interface overlay errors\. Verify Promise selection, await dependency logic, concurrency limiting, asynchronous fallback and pending request termination logic to eliminate timing bugs and zombie callbacks\.

- **Data Abnormality Inspection**: Target data disorder, state pollution and cache exceptions\. Check deep/shallow copy misuse, implicit array mutation, missing null fallback, uncaught NaN/Infinity, missing cache expiration and arbitrary global state modification\.

- **Engineering Deployment Inspection**: Check environment configuration mixing, invalid static cache strategy, abnormal cross\-origin preflight, residual redundant packages, mismatched CDN/resource paths and non\-standard Nginx/PM2 configurations causing online access exceptions\.

- **Back\-End Interface Inspection**: Check req/res reuse, missing interface timeout interception, undisclosed log desensitization, exposed error stacks, missing batch operation transactions and excessive request body issues causing interface timeout, leakage and exceptions\.

- **Database SQL Inspection**: Focus on SQL stuttering, deadlocks and data inconsistency\. Check index failure, deep pagination, unindexed sorting, excessive IN parameters, redundant large field queries, nested transactions and pessimistic lock abuse\.

- **General Troubleshooting Criteria**: Follow the process: Phenomenon positioning → Minimum snippet locking → Accurate verification → Targeted repair\. Prohibit full scanning, invalid verification and redundant analysis to save token and improve repair efficiency\.

---

## VIII\. AI Mandatory Production\-Level Self\-Inspection \&amp; Repair Process \(Final Barrier\)

After all code generation, modification, refactoring and fixing, AI must automatically execute full\-dimensional production self\-inspection without user instructions\. Verify compliance with all specification rules covering front\-end, back\-end, database, engineering deployment, security and performance, automatically repair all non\-compliant items, and output fully production\-deployable code\.

1. **Syntax \&amp; Basic Specification Self\-Inspection**: Verify variable declaration, equality judgment, syntax standardization, naming rules, code lines and single responsibility\. Eliminate low\-level syntax bugs, non\-standard writing and messy redundant code\.

2. **Security \&amp; Data Self\-Inspection**: Check hardcoded sensitive information, SQL injection risks, global/prototype pollution, log leakage, data desensitization missing, illegal values and null fallback missing\. Repair all security and data risks\.

3. **Asynchronous \&amp; Timing Self\-Inspection**: Verify rational Promise selection, asynchronous concurrency limiting, complete exception capture and request termination logic\. Eliminate silent asynchronous failures, timing disorder and interface accumulation\.

4. **Memory \&amp; Lifecycle Self\-Inspection**: Fully verify resource closed\-loop, focus on complete destruction of timers, event listeners, asynchronous requests, third\-party instances and KeepAlive cached components to completely eliminate memory leaks and zombie logic\.

5. **Business \&amp; Performance Self\-Inspection**: Verify rendering performance, index validity, pagination/sorting rationality, packaging optimization, cache strategy and interface layering\. Repair performance redundancy, scenario misuse and inefficient logic\.

6. **Engineering \&amp; Deployment Self\-Inspection**: Verify environment isolation, packaging configuration, Nginx/PM2 specification, cross\-origin configuration and resource path validity\. Eliminate online deployment errors, version update failures and resource 404 issues\.

7. **Final Standardized Repair**: Automatically fix all non\-compliant items, unify code style, comment specification and return format\. Ensure final code meets the production standard of**zero bugs, zero leaks, zero redundancy, ready for online deployment**\.

---

## IX\. Fixed Lock Rules \(Solve Long\-Term Conversation Rule Forgetting\)

**Initialization Lock Command**: Activate full production\-level engineering specifications for current conversation\. All code generation, modification, optimization and troubleshooting take this skill as the highest standard, abandon all AI default demo generation rules\.

**Lightweight Refresh Command**: Reset coding specification cognition, strictly execute all engineering, security, memory and scenario adaptation rules, prohibit rule degradation and logic regression\.

**Mandatory Self\-Inspection Command**: Verify current code in full compliance with specifications, automatically repair all engineering vulnerabilities and non\-standard writing, output final online\-ready version\.

> （注：文档部分内容可能由 AI 生成）
