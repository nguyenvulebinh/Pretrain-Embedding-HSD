# [VLSP2019-Hate Speech Detection Task] Register for using pre-trained embeddings

### Text for train embedding

- Data from [HSD task](http://vlsp.org.vn/vlsp2019)
- Data crawl from social network (Facebook)


### Type word embedding 

- CBOW word
- CBOW BPE word piece
- [Roberta](https://github.com/pytorch/fairseq/blob/master/examples/roberta/README.pretraining.md)

### Load word2vec using pickle

```python
import pickle

w2v_dict = pickle.load(open('./dict_map_comment.pkl', 'rb'))
print(w2v_dict['comment']['hello'].shape)
# (200,)
print(w2v_dict['comment_bpe']['hello'].shape)
# (200,)
```

