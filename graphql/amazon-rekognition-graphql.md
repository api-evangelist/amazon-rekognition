# Amazon Rekognition GraphQL Schema

This directory contains a conceptual GraphQL schema for the Amazon Rekognition API. The schema is derived from the Amazon Rekognition REST API and its public documentation at https://docs.aws.amazon.com/rekognition/latest/APIReference/.

Amazon Rekognition is a cloud-based computer vision service that provides deep-learning-powered image and video analysis. It exposes a JSON-over-HTTP REST API; this GraphQL schema represents the same surface area in a typed, graph-oriented form that can be used for documentation, tooling, mock servers, or as an adapter layer.

## Schema File

- `amazon-rekognition-schema.graphql` — Full GraphQL SDL schema covering image analysis, facial recognition, celebrity detection, content moderation, text detection, protective equipment detection, video analysis, streaming video, Custom Labels, face collections, media analysis, and face liveness.

## Type Coverage

The schema defines the following named types:

### Scalars
- `AWSDateTime` — ISO 8601 timestamps
- `AWSJSON` — arbitrary JSON values (e.g., tag maps)
- `Long` — 64-bit integers for timestamps and frame indices

### Enums
`GenderType`, `EmotionName`, `Attribute`, `OrientationCorrection`, `TextTypes`, `JobStatus`, `QualityFilter`, `BodyPart`, `ProtectiveEquipmentType`, `LandmarkType`, `ContentModerationSortBy`, `FaceSearchSortBy`, `LabelDetectionSortBy`, `PersonTrackingSortBy`, `SegmentType`, `TechnicalCueType`, `StreamProcessorStatus`, `DatasetType`, `ProjectStatus`, `ProjectVersionStatus`, `MediaAnalysisJobStatus`

### Geometry
`BoundingBox`, `Point`, `Polygon`, `Geometry`

### Image
`Image`, `ImageDetail`, `ImageQuality`, `DominantColor`, `S3Object`, `Bytes`

### Face Analysis
`AgeRange`, `Smile`, `Eyeglasses`, `Sunglasses`, `Gender`, `Beard`, `Mustache`, `EyeOpen`, `MouthOpen`, `FaceEmotion`, `FacePose`, `FaceQuality`, `Landmark`, `EyeDirection`, `FaceAttributes`, `FaceDetail`, `FaceOccluded`, `Face`, `FaceMatch`, `FaceMatchResult`, `ComparedSourceImageFace`, `CompareFacesMatch`, `ComparedFace`, `FaceSearchResult`, `IndexFacesResult`, `FaceRecord`, `UnindexedFace`

### Labels and Object Detection
`LabelCategory`, `LabelInstance`, `Label`, `LabelAlias`

### Celebrity Recognition
`CelebrityUrls`, `Celebrity`, `CelebrityDetail`, `KnownGender`, `RecognizedCelebrity`, `RecognizeCelebritiesResult`

### Content Moderation
`ModerationLabel`, `ContentModeration`, `ContentType`

### Text Detection
`TextDetection`, `TextBlock`

### Person and Body
`PersonDetail`, `PersonBody`, `HumanPart`, `BodyParts`

### Protective Equipment
`ProtectiveEquipment`, `ProtectiveEquipmentBodyPart`, `EquipmentDetection`, `CoversBodyPart`, `EquipmentType`

### Video Analysis
`Video`, `VideoDetail`, `NotificationChannel`, `StartJobResult`, `GetJobResult`, `Warning`, `Section`

### Stream Processors
`StreamProcessorInput`, `KinesisVideoStream`, `StreamProcessorOutput`, `KinesisDataStream`, `S3Destination`, `StreamProcessorSettings`, `FaceSearchSettings`, `StreamProcessor`, `StreamProcessorNotificationChannel`, `RegionOfInterest`, `StreamProcessorDataSharingPreference`

### Connected Home
`ConnectedHomeSettings`, `ConnectedHome`, `ConnectedDevice`

### Face Collections
`Collection`, `CollectionDetail`

### Video Segments
`SegmentDetection`, `TechnicalCue`, `TechnicalCueSegment`, `Shot`, `ShotSegment`

### Media Analysis
`MediaAnalysisInput`, `MediaAnalysisOperationsConfig`, `DetectModerationLabelsConfig`, `MediaAnalysisOutputConfig`, `MediaAnalysis`, `MediaAnalysisJobFailureDetails`, `MediaAnalysisResults`, `MediaAnalysisModelVersions`, `MediaAnalysisManifestSummary`

### Custom Labels / Projects
`Project`, `ProjectVersion`, `OutputConfig`, `TrainingDataResult`, `TestingDataResult`, `TrainingData`, `TestingData`, `ValidationData`, `Asset`, `GroundTruthManifest`, `EvaluationResult`, `Summary`, `DatasetMetadata`, `DatasetStats`

### Auth / Sessions
`APIKey`, `Token`

### Additional Result Types
`FaceLivenessSessionResult`, `LivenessOutputImage`, `AssociateFacesResult`, `AssociatedFace`, `UnsuccessfulFaceAssociation`, `DisassociateFacesResult`, `DisassociatedFace`, `UnsuccessfulFaceDisassociation`

## Query Operations

The `Query` type covers all read operations:

- `detectLabels` — object and scene detection in images
- `detectFaces` — face detection with optional attributes
- `compareFaces` — source-to-target face comparison
- `recognizeCelebrities` — celebrity identification in images
- `detectText` — OCR text extraction from images
- `detectModerationLabels` — unsafe content detection in images
- `searchFacesByImage` — search a collection using an image
- `searchFaces` — search a collection using a face ID
- `listCollections` / `describeCollection` / `listFaces` — collection management reads
- `detectProtectiveEquipment` — PPE detection on persons
- `detectCustomLabels` — custom-trained model inference
- `getLabelDetection` / `getFaceDetection` / `getCelebrityRecognition` / `getContentModeration` / `getPersonTracking` / `getTextDetection` / `getSegmentDetection` — async video job results
- `getFaceLivenessSessionResults` — liveness session result
- `describeStreamProcessor` / `listStreamProcessors` — stream processor reads
- `describeProjects` / `describeProjectVersions` — Custom Labels project reads
- `getMediaAnalysisJob` / `listMediaAnalysisJobs` — media analysis job reads
- `getImageProperties` — image quality and dominant color analysis

## Mutation Operations

The `Mutation` type covers all write and async-start operations:

- Collection management: `createCollection`, `deleteCollection`, `indexFaces`, `deleteFaces`
- User management: `createUser`, `deleteUser`, `associateFaces`, `disassociateFaces`
- Async video jobs: `startLabelDetection`, `startFaceDetection`, `startCelebrityRecognition`, `startContentModeration`, `startPersonTracking`, `startTextDetection`, `startSegmentDetection`, `startFaceSearch`
- Face liveness: `createFaceLivenessSession`
- Stream processors: `createStreamProcessor`, `deleteStreamProcessor`, `startStreamProcessor`, `stopStreamProcessor`, `updateStreamProcessor`
- Custom Labels projects: `createProject`, `deleteProject`, `createDataset`, `deleteDataset`, `createProjectVersion`, `stopProjectVersion`, `deleteProjectVersion`
- Media analysis: `startMediaAnalysisJob`
- Tagging: `tagResource`, `untagResource`

## References

- API Reference: https://docs.aws.amazon.com/rekognition/latest/APIReference/
- Developer Guide: https://docs.aws.amazon.com/rekognition/latest/dg/what-is.html
- Service Home: https://aws.amazon.com/rekognition/
