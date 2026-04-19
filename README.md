# Amazon Rekognition (amazon-rekognition)
Amazon Rekognition is a cloud-based computer vision service that makes it easy to add image and video analysis to your applications, providing capabilities such as object and scene detection, facial analysis, face comparison, celebrity recognition, text detection, content moderation, custom labels, face liveness detection, and streaming video analysis using deep learning technology.

**URL:** [Visit Amazon Rekognition](https://aws.amazon.com/rekognition/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - AWS, Celebrity Recognition, Computer Vision, Content Moderation, Custom Labels, Deep Learning, Face Liveness, Facial Recognition, Image Analysis, Machine Learning, Object Detection, Text Detection, Video Analysis

## Timestamps

- **Created:** 2024-01-15
- **Modified:** 2026-04-19

## APIs

### Amazon Rekognition
Amazon Rekognition provides image and video analysis APIs for label detection, facial analysis, face comparison, celebrity recognition, text detection, content moderation, custom labels, face liveness detection, and streaming video analysis.

**Human URL:** [https://aws.amazon.com/rekognition/](https://aws.amazon.com/rekognition/)

#### Tags

 - Computer Vision, Image Analysis, Video Analysis, Facial Recognition, Machine Learning

#### Properties

- [Documentation](https://docs.aws.amazon.com/rekognition/latest/dg/what-is.html)
- [OpenAPI](openapi/amazon-rekognition-openapi.yml)
- [APIReference](https://docs.aws.amazon.com/rekognition/latest/APIReference/Welcome.html)
- [GettingStarted](https://docs.aws.amazon.com/rekognition/latest/dg/getting-started.html)
- [Authentication](https://docs.aws.amazon.com/rekognition/latest/dg/security_iam_service-with-iam.html)
- [Pricing](https://aws.amazon.com/rekognition/pricing/)
- [FAQ](https://aws.amazon.com/rekognition/faqs/)

## Common Properties

- [Portal](https://aws.amazon.com/)
- [DeveloperPortal](https://aws.amazon.com/rekognition/)
- [Documentation](https://docs.aws.amazon.com/rekognition/)
- [Console](https://console.aws.amazon.com/rekognition/)
- [SignUp](https://portal.aws.amazon.com/billing/signup)
- [Pricing](https://aws.amazon.com/rekognition/pricing/)
- [TermsOfService](https://aws.amazon.com/service-terms/)
- [PrivacyPolicy](https://aws.amazon.com/privacy/)
- [Support](https://aws.amazon.com/support/)
- [Blog](https://aws.amazon.com/blogs/machine-learning/)
- [GitHubOrganization](https://github.com/aws)
- [StatusPage](https://health.aws.amazon.com/health/status)
- [YouTube](https://www.youtube.com/user/AmazonWebServices)
- [StackOverflow](https://stackoverflow.com/questions/tagged/amazon-rekognition)

## Features

| Name | Description |
|------|-------------|
| Object and Scene Detection | Detect thousands of objects, scenes, and concepts in images and videos with high confidence scores using deep learning. |
| Facial Analysis | Detect and analyze faces with attributes including age range, emotions, gender, and facial landmarks. |
| Face Comparison | Compare faces across images to determine if they are the same person with a similarity score. |
| Face Collections | Create searchable face collections to index and search millions of faces in near real-time. |
| Celebrity Recognition | Identify thousands of celebrities in images and videos across categories like sports, entertainment, and politics. |
| Text Detection | Detect and extract printed and handwritten text from images and videos in multiple languages. |
| Content Moderation | Detect explicit, inappropriate, or violent content in images and videos for automated content moderation. |
| Custom Labels | Build and train custom image classifiers using your own labeled images for domain-specific object detection. |
| Protective Equipment Detection | Detect personal protective equipment such as face covers, hand covers, and head covers on persons in images. |
| Face Liveness Detection | Verify that a user is physically present during identity verification to prevent spoofing attacks. |
| People Pathing | Track and follow identified people across frames in stored video footage. |
| Video Segmentation | Identify technical cues and segments such as black frames, end credits, and color bars in video content. |
| Streaming Video Analysis | Analyze live streaming video in real-time using Amazon Kinesis Video Streams integration. |
| Image Properties Analysis | Evaluate image quality attributes including sharpness, brightness, contrast, and dominant colors. |

## Use Cases

| Name | Description |
|------|-------------|
| Identity Verification | Verify user identities by comparing selfies to ID documents or previously stored face images for onboarding and authentication. |
| Content Moderation | Automatically moderate user-generated content on platforms to detect and filter explicit or inappropriate imagery. |
| Searchable Media Libraries | Build searchable image and video archives by automatically tagging media with detected labels, faces, and text. |
| Workplace Safety Compliance | Monitor camera feeds to detect whether workers are wearing required personal protective equipment in industrial settings. |
| Fraud Prevention | Prevent identity fraud during digital onboarding by using face liveness detection to confirm real users. |
| Smart Retail Analytics | Analyze in-store camera feeds to track customer behavior, measure foot traffic, and optimize product placement. |
| Public Safety and Security | Search video archives for persons of interest by comparing faces against a known collection. |
| Media and Entertainment | Automatically tag celebrities in photos and videos for media companies to improve content discoverability. |
| Custom Object Detection | Train custom classifiers to detect proprietary products, logos, brand assets, or industry-specific objects. |

## Integrations

| Name | Description |
|------|-------------|
| Amazon S3 | Process images and videos stored in Amazon S3 buckets directly without downloading content. |
| Amazon Kinesis Video Streams | Analyze live video streams in real-time by integrating with Kinesis Video Streams for streaming analysis. |
| AWS Lambda | Trigger serverless analysis pipelines by invoking Rekognition from Lambda functions in event-driven architectures. |
| Amazon SNS | Receive asynchronous notifications when stored video analysis jobs complete via Amazon SNS. |
| AWS IAM | Control access to Rekognition APIs using AWS Identity and Access Management policies and roles. |
| Amazon CloudWatch | Monitor Rekognition API usage, latency, and error metrics through CloudWatch dashboards and alarms. |
| AWS Step Functions | Orchestrate multi-step computer vision workflows using Step Functions to chain Rekognition operations. |
| Amazon Augmented AI (A2I) | Route low-confidence Rekognition predictions to human reviewers using Amazon Augmented AI for quality control. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [amazon-rekognition-openapi.yml](openapi/amazon-rekognition-openapi.yml)

### JSON Schema

- [amazon-rekognition-bounding-box-schema.json](json-schema/amazon-rekognition-bounding-box-schema.json)
- [amazon-rekognition-compare-faces-request-schema.json](json-schema/amazon-rekognition-compare-faces-request-schema.json)
- [amazon-rekognition-compare-faces-response-schema.json](json-schema/amazon-rekognition-compare-faces-response-schema.json)
- [amazon-rekognition-create-collection-request-schema.json](json-schema/amazon-rekognition-create-collection-request-schema.json)
- [amazon-rekognition-create-collection-response-schema.json](json-schema/amazon-rekognition-create-collection-response-schema.json)
- [amazon-rekognition-create-face-liveness-session-request-schema.json](json-schema/amazon-rekognition-create-face-liveness-session-request-schema.json)
- [amazon-rekognition-create-face-liveness-session-response-schema.json](json-schema/amazon-rekognition-create-face-liveness-session-response-schema.json)
- [amazon-rekognition-detect-custom-labels-request-schema.json](json-schema/amazon-rekognition-detect-custom-labels-request-schema.json)
- [amazon-rekognition-detect-custom-labels-response-schema.json](json-schema/amazon-rekognition-detect-custom-labels-response-schema.json)
- [amazon-rekognition-detect-faces-request-schema.json](json-schema/amazon-rekognition-detect-faces-request-schema.json)
- ...and 26 more

### JSON Structure

- [amazon-rekognition-bounding-box-structure.json](json-structure/amazon-rekognition-bounding-box-structure.json)
- [amazon-rekognition-compare-faces-request-structure.json](json-structure/amazon-rekognition-compare-faces-request-structure.json)
- [amazon-rekognition-compare-faces-response-structure.json](json-structure/amazon-rekognition-compare-faces-response-structure.json)
- [amazon-rekognition-create-collection-request-structure.json](json-structure/amazon-rekognition-create-collection-request-structure.json)
- [amazon-rekognition-create-collection-response-structure.json](json-structure/amazon-rekognition-create-collection-response-structure.json)
- [amazon-rekognition-create-face-liveness-session-request-structure.json](json-structure/amazon-rekognition-create-face-liveness-session-request-structure.json)
- [amazon-rekognition-create-face-liveness-session-response-structure.json](json-structure/amazon-rekognition-create-face-liveness-session-response-structure.json)
- [amazon-rekognition-detect-custom-labels-request-structure.json](json-structure/amazon-rekognition-detect-custom-labels-request-structure.json)
- [amazon-rekognition-detect-custom-labels-response-structure.json](json-structure/amazon-rekognition-detect-custom-labels-response-structure.json)
- [amazon-rekognition-detect-faces-request-structure.json](json-structure/amazon-rekognition-detect-faces-request-structure.json)
- ...and 26 more

### JSON-LD

- [amazon-rekognition-context.jsonld](json-ld/amazon-rekognition-context.jsonld)

### Examples

- [amazon-rekognition-bounding-box-example.json](examples/amazon-rekognition-bounding-box-example.json)
- [amazon-rekognition-compare-faces-request-example.json](examples/amazon-rekognition-compare-faces-request-example.json)
- [amazon-rekognition-compare-faces-response-example.json](examples/amazon-rekognition-compare-faces-response-example.json)
- [amazon-rekognition-create-collection-request-example.json](examples/amazon-rekognition-create-collection-request-example.json)
- [amazon-rekognition-create-collection-response-example.json](examples/amazon-rekognition-create-collection-response-example.json)
- [amazon-rekognition-create-face-liveness-session-request-example.json](examples/amazon-rekognition-create-face-liveness-session-request-example.json)
- [amazon-rekognition-create-face-liveness-session-response-example.json](examples/amazon-rekognition-create-face-liveness-session-response-example.json)
- [amazon-rekognition-detect-custom-labels-request-example.json](examples/amazon-rekognition-detect-custom-labels-request-example.json)
- [amazon-rekognition-detect-custom-labels-response-example.json](examples/amazon-rekognition-detect-custom-labels-response-example.json)
- [amazon-rekognition-detect-faces-request-example.json](examples/amazon-rekognition-detect-faces-request-example.json)
- ...and 26 more

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Amazon Rekognition](capabilities/shared/rekognition.yaml) — 15 operations for image analysis, facial recognition, video analysis, and face liveness

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Computer Vision Workflows](capabilities/computer-vision-workflows.yaml) | rekognition | 15 | Application Developer, Security Engineer, Content Moderator |

## Vocabulary

- [Amazon Rekognition Vocabulary](vocabulary/amazon-rekognition-vocabulary.yaml) — Unified taxonomy mapping 12 resources, 11 actions, 1 workflow, and 3 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Amazon Rekognition Spectral Rules](rules/amazon-rekognition-spectral-rules.yml) — 19 rules across 6 categories enforcing Amazon Rekognition API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
