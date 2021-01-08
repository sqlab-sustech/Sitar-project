## Sitar-project

This repository contains the artifacts in the Sitar project.

### Co-Evolution Samples in Dubbo and Kafka

See the directory [dubbo-kafka](dubbo-kafka).

#### Explaination of files

+ [dubbo_coevo_patches.txt](dubbo-kafka/dubbo_coevo_patches.txt): Co-evolution patches in [Duboo](https://github.com/apache/dubbo).

+ [kafka_coevo_patches.txt](dubbo-kafka/kafka_coevo_patches.txt): Co-evolution patches in [Kafka](https://github.com/apache/kafka).

+ [special_dubbo_kafka.txt](dubbo-kafka/special_dubbo_kafka.txt): uncommon co-evolution patches in Dubbo and Kafka.

#### Data related to empirical study

The co-evolution change type is already labeled in the text file.

To get the timestamp of commit A (A is SHA1 digest), use the following command in the git repository:

```bash
git show -s --format=%cI A
```

To obtain the number of commits between A and B (A and B are SHA1 digests), use the following command:

```bash
git rev-list --count A..B
```

---

### Samples with Manual Inspection Results

See the directory [co-evolution-samples](co-evolution-samples).

#### File list

+ [negative list](co-evolution-samples/negative): Negative sample patches (not co-evolved in **20 days**).

+ [positive list](co-evolution-samples/positive): Positive sample patches (co-evolved in **2 days**).

+ [negative-findings.xlsx](co-evolution-samples/negative-findings.xlsx): Inspecting results of *negative samples*.

+ [positive-findings.xlsx](co-evolution-samples/positive-findings.xlsx): Inspecting results of *positive samples*.

---

### Empirical data

The data used in empirical study is under [empirical_data](empirical_data) directory.
Some repositories do not contain co-evolution changes thus are removed.

---

### Experiment data

The data used in experiment is under [experiment_data](experiment_data) directory.
